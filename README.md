# git-tutorial

> [!WARNING]  
> The `task_ans` branch contains answers for `task`. To ensure effective learning and prevent easy access, delete this branch before giving out the tasks.


### Instructions
Follow the tasks below to test your Git knowledge. Perform each step as specified and answer the questions accordingly.

1. Create a new branch from `task` named `b_<username>`

   - Question: What command did you use to create and switch to the new branch?

     <details>
     <summary>Answer</summary>

     ```sh
     git checkout task
     git checkout -b b_<username>
     # or
     git checkout -b b_<username> task
     ```
     </details>

2. Create a folder named `f_<username>` in the `task` folder with a file named `<username>.txt` containing the text `Hello Git!`

   - Question: What command did you use to create the folder and the file?

     <details>
     <summary>Answer</summary>

     ```sh
     mkdir task/f_<username>
     echo "Hello Git!" > task/f_<username>/<username>.txt
     ```
     </details>

3. Stage and commit the changes with the commit message `init(<branch_name>): set up git tutorial task content`

   - Question: What was the exact commit command used?

     <details>
     <summary>Answer</summary>

     ```sh
     git add .
     git commit -m "init(b_<username>): set up git tutorial task content"
     ```
     </details>

4. Send a pull request to the `task` branch

   - Question: Which steps did you take on GitHub to create the pull request?

     <details>
     <summary>Answer</summary>

     1. Push your branch to the remote repository

        ```sh
        git push -u origin b_<username>
        ```

     2. Go to your repository on GitHub
     3. Click on `Compare & pull request`
     4. Ensure the base branch is `task` and the compare branch is `b_<username>`
     5. Add a title and description for the pull request, then click `Create pull request`
     </details>

5. Wait for merging

   - Question: How will you know when your pull request has been successfully merged?

     <details>
     <summary>Answer</summary>

     - You will see a message indicating that the pull request has been merged on GitHub, and the branch will be marked as merged
     - You may also receive a notification via email or GitHub notifications if enabled
     </details>

6. Delete your branch after merging

   - Question: What command did you use to delete your branch after merging?

     <details>
     <summary>Answer</summary>

     ```sh
     # delete the branch locally
     git branch -d b_<username>

     # delete the branch from the remote repository
     git push origin -d b_<username>
     ```
     </details>