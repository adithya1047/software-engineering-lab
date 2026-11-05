# Test Cases

| TC ID | Task | Objective | Test Steps (Input) | Expected Result | Verification | Status |
|---|---|---|---|---|---|---|
| TC01 | 1 | Check whether git init creates a repository | Run `git init` | A new Git repository should be created | Automated | Pass |
| TC02 | 2 | Check git status | Run `git status` and create a new file | Git should show tracked and untracked files | Manual | Pass |
| TC03 | 3 | Check git add | Create a file and run `git add notes.txt` | File should be added to staging area | Manual | Pass |
| TC04 | 4 | Check git commit | Run `git commit -m "Add notes"` | Changes should be saved as a commit | Automated | Pass |
| TC05 | 5 | Check git log | Run `git log` and `git log --oneline` | Complete commit history should be displayed | Manual | Pass |
| TC06 | 6 | Check git diff | Modify a file and run `git diff` | Differences between modified and original file should appear | Manual | Pass |
| TC07 | 7 | Check git diff --staged | Modify a file, stage it and run `git diff --staged` | Staged changes should be displayed | Manual | Pass |
| TC08 | 8 | Check git commit --amend | Make a commit and modify it using `git commit --amend` | Latest commit message and hash should be updated | Manual | Pass |
| TC09 | 9 | Check branch creation | Run `git branch scratch` | A new branch named scratch should be created | Automated | Pass |
| TC10 | 10 | Check branch switching | Run `git switch scratch` and `git switch main` | User should be able to switch between branches | Manual | Pass |
| TC11 | 11 | Check fast-forward merge | Create a commit in another branch and merge it into main | Changes should be merged successfully | Automated | Pass |
| TC12 | 12 | Check merge conflict resolution | Merge two branches with conflicting changes and resolve them | Conflict should be resolved and merge commit created | Automated | Pass |
| TC13 | 13 | Check git restore | Modify a file and run `git restore about.txt` | Unstaged changes should be discarded | Manual | Pass |
| TC14 | 14 | Check git restore --staged | Stage a modified file and run `git restore --staged` | File should be removed from staging without losing changes | Manual | Pass |
| TC15 | 15 | Check git reset --soft | Run `git reset --soft HEAD~1` | Latest commit should be removed but changes should remain staged | Manual | Pass |
| TC16 | 16 | Check git reset --mixed | Run `git reset --mixed HEAD~1` | Commit should be removed and changes should become unstaged | Manual | Pass |
| TC17 | 17 | Check git reset --hard | Run `git reset --hard HEAD~1` | Latest commit and its changes should be discarded | Manual | Pass |
| TC18 | 18 | Check git revert | Run `git revert` with a commit hash | A new commit should be created to undo previous changes | Automated | Pass |
| TC19 | 19 | Check git stash and stash pop | Modify a file, run `git stash` and then `git stash pop` | Changes should be temporarily stored and restored | Manual | Pass |
| TC20 | 20 | Check git clone | Run `git clone` with a repository path | A local copy of the repository should be created | Automated | Pass |
| TC21 | 21 | Check git log filters | Run `git log --author`, `git log --grep` and `git log -n 3` | Commits should be filtered according to the given conditions | Manual | Pass |
| TC22 | 22 | Check git log -S | Search for a particular text using `git log -S` | Git should identify commits that introduced or removed the text | Automated | Pass |
| TC23 | 23 | Check git bisect | Run `git bisect` to identify a faulty commit | Git should identify the first commit that introduced the error | Automated | Pass |
| TC24 | 24 | Check git blame | Run `git blame about.txt` | Author and commit information for each line should be displayed | Manual | Pass |
| TC25 | 25 | Check git show | Run `git show` with a commit hash | Details and changes of the selected commit should appear | Manual | Pass |
| TC26 | 26 | Check git tag | Create lightweight and annotated tags | Both tags should be created and displayed | Automated | Pass |
| TC27 | 27 | Check git remote | Run `git remote -v` and add a backup remote | Remote repository details should be displayed correctly | Automated | Pass |
| TC28 | 28 | Check git push | Run `git push origin feature/loyalty-card` | Local branch should be uploaded to the remote repository | Automated | Pass |
| TC29 | 29 | Check git pull | Run `git pull origin main` | Latest remote changes should be downloaded and merged | Automated | Pass |
| TC30 | 30 | Check git fetch | Run `git fetch origin` | Remote changes should be downloaded without merging | Automated | Pass |
| TC31 | 31 | Check git cherry-pick | Run `git cherry-pick` with a commit hash | Selected commit changes should be applied to the current branch | Automated | Pass |
| TC32 | 32 | Check interactive rebase | Run `git rebase -i HEAD~3` and squash commits | Multiple commits should be combined into one commit | Automated | Pass |
| TC33 | 33 | Check git rebase | Run `git rebase main` from a feature branch | Feature branch should be updated with main branch history | Manual | Pass |
| TC34 | 34 | Check git reflog | Run `git reflog` and create a branch from a recovered commit | Previous commit should be recovered successfully | Automated | Pass |
| TC35 | 35 | Check conflict resolution during rebase | Run `git rebase main` and resolve conflicts | Rebase should complete without conflicts | Automated | Pass |
| TC36 | 36 | Check .gitignore and git rm --cached | Add a file to `.gitignore` and run `git rm --cached` | File should remain on disk but stop being tracked by Git | Automated | Pass |
| TC37 | 37 | Check git diff between branches | Run `git diff branchA..branchB` | Differences between the two branches should be displayed | Manual | Pass |
| TC38 | 38 | Check detached HEAD | Checkout an old commit, create a new commit and save it using a new branch | New branch should preserve the experimental commit | Manual | Pass |

## Summary

| Metric | Value |
|---|---|
| Total Test Cases | 38 |
| Automated | 18 |
| Manual | 20 |
| Passed | 38 |
| Failed | 0 |
