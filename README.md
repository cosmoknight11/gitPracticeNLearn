# gitPracticeNLearn
## ALl the necesary notes here.

* Scenario 1: Cloning a Repo, Making Changes, but Want to Discard Them and Get Latest Updates
    - git fetch origin: to get the head of the remote repo, if thats ahead f current
    - git pull origin <branch-name> : to pull the origin.To the current repo
* Scenario 2: Cloning a Repo, Committing Locally, but Want to Discard Your Commit 
    - git reset --hard HEAD~1
* Scenario 3: Cloning a Repo, Committing Locally, but Want to Keep Your Commit While Pulling Latest Changes
    - git fetch origin
    - git rebase origin/<branch-name>
    - git rebase --continue
    - git push origin 
* Scenario 4: Stashing Changes to Pull Latest Code Without Committing
    - git stash
    - git pull origin <branch-name>
    - git stash pop
    - resolve merge conflits and commit
* Scenario 5: Deleting a Commit from Remote History:
    - git reset --hard HEAD~1
    - git push origin <branch-name> --force :Note: Be careful with --force as it rewrites history and can cause issues for teammates who have pulled the deleted commit.
* Scenario 6: Rewriting a Commit Message After Pushing to Remote
    - git commit --amend : opens editor for commit messagages
    - git push origin <branch-name> --force


