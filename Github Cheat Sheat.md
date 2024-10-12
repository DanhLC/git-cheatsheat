# This cheat sheet includes commonly used Git and GitHub commands to help you manage and work with repositories effectively.</p>

## 1. Set Up and Configure Git</h2>

### Set username

<pre><code>
git config --global user.name "Your Name"
</code></pre>

### Set email

<pre><code>
git config --global user.email "youremail@example.com"
</code></pre>

### Check configuration

<pre><code>
git config --list
</code></pre>

## 2. Create and Manage Repositories

### Initialize a new repository

<pre><code>
git init
</code></pre>

### Clone a repository from GitHub

<pre><code>
git clone https://github.com/user/repository.git
</code></pre>

## 3. Status and Information</h2>

### Check the status of your repository        

<pre><code>
git status
</code></pre>

### View commit history

<pre><code>
git log
</code></pre>

### View a short log history

<pre><code>
git log --oneline
</code></pre>

## 4. Working with Files

### Add new or modified files to staging area

<pre><code>
git add <file>
</code></pre>

### Add all files to staging area

<pre><code>
git add .
</code></pre>

### Remove a file from staging area

<pre><code>
git reset <file>
</code></pre>

### Delete a file from both working directory and staging area

<pre><code>
git rm <file>
</code></pre>

### Move or rename a file

<pre><code>
git mv <old_filename> <new_filename>
</code></pre>

## 5. Commit Changes</h2>

### Create a commit with a message

<pre><code>
git commit -m "Commit message"
</code></pre>

### Commit and include unstaged changes

<pre><code>
git commit -a -m "Commit message"
</code></pre>

## 6. Branching</h2>

### Create a new branch

<pre><code>
git branch <branch_name>
</code></pre>

### List branches

<pre><code>
git branch
</code></pre>

### Switch branches

<pre><code>
git checkout <branch_name>
</code></pre>

### Create and switch to a new branch

<pre><code>
git checkout -b <branch_name>
</code></pre>

### Merge a branch into the current branch

<pre><code>
git merge <branch_name>
</code></pre>

### Delete a branch

<pre><code>
git branch -d <branch_name>
</code></pre>

## 7. Remote Operations

### List remotes

<pre><code>
git remote -v
</code></pre>

### Add a new remote

<pre><code>
git remote add origin https://github.com/user/repository.git
</code></pre>

### Remove a remote

<pre><code>
git remote remove <remote_name>
</code></pre>

### Fetch changes from remote without merging

<pre><code>
git fetch origin
</code></pre>

### Pull changes from remote and merge

<pre><code>
git pull origin <branch_name>
</code></pre>

### Push changes to remote

<pre><code>
git push origin <branch_name>
</code></pre

## 8. Undoing Changes</h2>

### Revert file to the last commit

<pre><code>
git checkout -- <file>
</code></pre

### Undo the last commit but keep changes

<pre><code>
git reset --soft HEAD~1
</code></pre

### Undo the last commit and discard changes

<pre><code>
git reset --hard HEAD~1
</code></pre

## 9. Tags

### Create a new tag

<pre><code>
git tag <tag_name>
</code></pre>

### List all tags

<pre><code>
git tag
</code></pre>

### Delete a tag

<pre><code>
git tag -d <tag_name>
</code></pre>

### Push tags to remote

<pre><code>
git push origin --tags
</code></pre>

## 10. Rebase</h2>

### Rebase the current branch onto another branch

<pre><code>
git rebase <branch_name>
</code></pre>

### Abort a rebase

<pre><code>
git rebase --abort
</code></pre>

## 11. Stashing</h2>

### Stash current changes

<pre><code>
git stash
</code></pre>

### Apply the stashed changes

<pre><code>
git stash pop
</code></pre>

### List all stashes

<pre><code>
git stash list
</code></pre>

### Drop a stash

<pre><code>
git stash drop
</code></pre>

## 12. Other Useful Commands</h2>

### View the change history of a file

<pre><code>
git log -- <file>
</code></pre>

### View differences between unstaged changes

<pre><code>
git diff
</code></pre>

### View differences between staged changes and the last commit

<pre><code>
git diff --staged
</code></pre>

Created by * DanhLC * - This Git and GitHub Cheat Sheet provides a quick reference to essential commands.
For more advanced usage, refer to the https://git-scm.com/doc Git documentation
