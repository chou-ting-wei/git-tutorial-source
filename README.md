# git-tutorial

### User Configuration

1. Set your identity
   ```sh
   git config --global user.name "your_name"
   git config --global user.email "your_email@example.com"
   ```
   > To keep your email address private, use your GitHub-provided `no-reply` email address.
2. Set default commit branch
   ```sh
   git config --global init.defaultBranch main
   ```
3. Check your settings
   ```sh
   git config --list
   ```

### SSH Key Setup

1. Generate a new SSH key
   ```sh
   ssh-keygen -t ed25519 -C "your_email@example.com"
   ```
2. Copy the SSH public key to your clipboard

   ```sh
   cat ~/.ssh/id_ed25519.pub
   ```

   > Then select and copy the contents of the `id_ed25519.pub` file displayed in the terminal to your clipboard.

3. Add a new SSH authentication key to your account

### Basic Operations

1. Clone a repository
   ```sh
   git clone <repository_url>
   ```
2. Pull changes from the remote repository
   ```sh
   git pull
   ```
3. Stage files in the current directory

   ```sh
   # stage a specific file
   git add <file_name>

   # stage multiple specific files
   git add <file_name1> <file_name2>

   # stage all changes in the current directory
   git add .
   ```

4. Commit your changes
   ```sh
   git commit -m "<commit_message>"
   ```
5. Push changes to the remote repository
   ```sh
   git push
   ```

### Branch Operations

1. Switch to an existing branch
   ```sh
   git checkout <branch_name>
   ```
2. Create a new branch from the current branch and switch to it
   ```sh
   git checkout -b <new_branch_name>
   ```
3. Create a new branch from a specific branch and switch to it
   ```sh
   git checkout -b <new_branch_name> <branch_name>
   ```
4. List all branches
   ```sh
   git branch
   ```
5. Rename the current branch
   ```sh
   git branch -m <new_branch_name>
   ```
6. Delete a local branch
   ```sh
   git branch -d <branch_name>
   ```
7. Push a new branch to the remote repository
   ```sh
   git push -u origin <branch_name>
   ```
8. Delete a branch from the remote repository
   ```sh
   git push origin -d <branch_name>
   ```

### Additional References

For more information, visit: [Git/GitHub | userwei's Note](https://note.userwei.com/docs/setup/tool/git/)
