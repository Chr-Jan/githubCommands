# GitHubs Commands

This cheat sheet is for easy access to Git commands when needed.

## Delete all commit history in GitHub

1. **Checkout/create orphan branch** (this branch won't show in `git branch` command):
    ```bash
    git checkout --orphan latest_branch
    ```

2. **Add all the files** to the newly created branch:
    ```bash
    git add -A
    ```

3. **Commit the changes**:
    ```bash
    git commit -am "commit message"
    ```

4. **Delete main (default) branch** (this step is permanent):
    ```bash
    git branch -D main
    ```

5. **Rename the current branch to main**:
    ```bash
    git branch -m main
    ```

6. **Force update your remote repository** to apply all changes:
    ```bash
    git push -f origin main
    ```
