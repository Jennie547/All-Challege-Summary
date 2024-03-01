# REANAME DEFAULT BRANCH

## To rename the default branch from "master" to "main" in a Git repository, you can follow these steps:

### Renaming the Branch Locally:

1. **Checkout the Current Branch**: Make sure you are on the branch you want to rename (usually "master").

   ```bash
   git checkout master
   ```

2. **Create a New Branch**: Create a new branch named "main" from the current branch.

   ```bash
   git branch -m main
   ```

3. **Push the New Branch**: Push the new "main" branch to the remote repository.

   ```bash
   git push -u origin main
   ```

### Updating the Default Branch on the Remote Repository:

1. **Change the Default Branch in the Remote Repository**: Go to your remote repository (e.g., GitHub) and navigate to the repository settings. Look for an option to change the default branch and set it to "main".

2. **Delete the Old Branch (Optional)**: If you no longer need the "master" branch, you can delete it both locally and on the remote repository.

   ```bash
   git branch -d master
   git push origin --delete master
   ```

### Updating Local Repositories:

If you have other local repositories that are clones of the original repository, you need to update their default branch settings as well. You can do this by fetching the changes from the remote repository and updating the default branch in each local repository.

### Note:

- Renaming the default branch may affect existing workflows or scripts that rely on the old branch name. Make sure to update any references to the branch name accordingly.
- Always make sure to have a backup of your repository before making significant changes like renaming the default branch.

By following these steps, you can rename the default branch from "master" to "main" in your Git repository.