# Hi — I’m rosamariacastellanoz060-ai

This is my GitHub profile README. Below is a recent open-source contribution I made.

## Recent contribution

**fix(editor): treat missing write capability as editable**
Contributed author on PR [Acode-Foundation/Acode#2853](https://github.com/Acode-Foundation/Acode/pull/2853) — merged 2026-09-03

What I changed
- Fixed file-read/write detection so files without an explicit write flag are treated as editable.
- Improved search progress handling to avoid showing 100% before completion.

Files changed: 2 — +4 / −3

File attributions
- src/lib/openFile.js
  - Original / main source: Ajit Kumar (deadlyjack) — https://github.com/deadlyjack
  - Finished / recent contributor for this change: Raunak Raj (bajrangCoder) — https://github.com/bajrangCoder

- src/sidebarApps/searchInFiles/index.js
  - Original / main source: Ajit Kumar (deadlyjack) — https://github.com/deadlyjack
  - Finished / recent contributor for this change: Raunak Raj (bajrangCoder) — https://github.com/bajrangCoder

Key change (robust read-only check):

```js
// before
const readOnly = fileInfo.canWrite ? false : true;
// after
const readOnly = fileInfo.canWrite === false;
```

Link: https://github.com/Acode-Foundation/Acode/pull/2853

Impact: prevents incorrectly marking files as read-only when write capability is missing; improves UX for editor and search progress.

---

If you want this written in a different tone (shorter, more formal, or more technical), tell me and I’ll update it.