# Exercise - Git Branching

#### **Objective:**
Learn to create, switch between, merge, and manage conflicts in Git branches.

#### **Setup:**

1. **Clone the assignment:**
   - Copy the git assignment url. Example `https://github.com/username/assignmenturl.git`
   - On a directory in your computer, run `git clone https://github.com/username/assignmenturl.git`

#### **Tasks:**

1. **Create and Switch to a New Branch:**
   - Create a new branch named `feature-add-about`:
     ```
     git branch feature-add-about
     ```
   - Switch to this branch:
     ```
     git switch feature-add-about
     ```

2. **Add a New File:**
   - In the `feature-add-about` branch, create a file called `ABOUT.txt`.
   - Add some content to `ABOUT.txt`, such as "This file contains information about the project."
   - Add and commit the changes:
     ```
     git add ABOUT.txt
     git commit -m "Add ABOUT.txt with project information"
     ```

3. **Merge Branch:**
   - Switch back to the main branch using:
     ```
     git switch main
     ```
   - Merge the `feature-add-about` branch into main:
     ```
     git merge feature-add-about
     ```
   - If there are no conflicts, finalize the merge. If there are conflicts, resolve them as instructed by Git.

4. **Handle Conflicts (Optional):**
   - For more practice, create another branch called `feature-update-about` and switch to it.
   - Make changes to `ABOUT.txt` in this new branch.
   - Switch back to main and make different changes to `ABOUT.txt`.
   - Try to merge `feature-update-about` into main and handle the merge conflict that arises.

5. **Push your changes:**
   - The changes you have made on the main branch are still on your local computer so we need to push it to GitHub.
   - Push your changes by running:
     ```
     git add .
     git commit -m "Finished exercise"
     git push
     ```

