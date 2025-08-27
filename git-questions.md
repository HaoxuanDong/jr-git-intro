## Git True/False Questions with Answers
### 1. 1.	Suppose you had a file, called first.md, and you made a copy of this file, named it second.md and made some changes to it. Next, suppose you ran diff -u first.md second.md.
**Answer:** AB$C#%EF

---
### 2. If you accidentally add a file to the staging area, you can remove it using `git reset`. For example, if you accidentally add `thrid.md`, but don’t want it to be committed yet, run `git reset thrid.md` and the file will be removed from the staging area, but it will still be in your working directory.  
**Answer:** True ✅  
- `git reset <file>` removes the file from the staging area but keeps it in the working directory.

---

### 3. The commands `git reset` and `git revert` can only be used to undo commits in the git repository.  
**Answer:** False ❌  
- `git reset` can also be used to unstage files (not only undo commits).  
- `git revert` is specifically for undoing commits by creating a new reverse commit.

---

### 4. The command `git checkout` can be used to roll back to a certain commit hash.  
**Answer:** True ✅  
- `git checkout <commit-hash>` allows you to switch to that commit in a “detached HEAD” state.

---

### 5. We cannot commit changes in the working directory directly to the repo without adding it to the staging index first.  
**Answer:** True ✅  
- You must stage changes before committing.  
- The exception is `git commit -a`, which automatically stages tracked files before committing.

---

### 6. `git log -p` and `git log` will give you the same output.  
**Answer:** False ❌  
- `git log` shows commit history.  
- `git log -p` shows commit history **plus diffs (patches)** for each commit.

---

### 7. `git log --oneline` and `git log --stat` will give you the same output.  
**Answer:** False ❌  
- `--oneline`: condensed commit hash + message.  
- `--stat`: commit info + summary of file changes (insertions/deletions).

---

### 8. It is recommended that in most cases we should use `git revert` rather than `git reset` to undo commits because `git revert` is safer.  
**Answer:** True ✅  
- `git revert` creates a new commit and does not rewrite history.  
- `git reset` rewrites commit history and may cause issues in shared repos.

---
