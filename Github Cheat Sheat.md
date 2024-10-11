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

## 4. Working with Files</h2>

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
git checkout <branch_name>

### Create and switch to a new branch
git checkout -b <branch_name>

### Merge a branch into the current branch
git merge <branch_name>

### Delete a branch
git branch -d <branch_name>
        </code></pre>
    </div>

    <div class="section">
        <h2>7. Remote Operations</h2>
        <pre><code># List remotes
git remote -v

### Add a new remote
git remote add origin https://github.com/user/repository.git

### Remove a remote
git remote remove <remote_name>

### Fetch changes from remote without merging
git fetch origin

### Pull changes from remote and merge
git pull origin <branch_name>

### Push changes to remote
git push origin <branch_name>
        </code></pre>
    </div>

    <div class="section">
        <h2>8. Undoing Changes</h2>
        <pre><code># Revert file to the last commit
git checkout -- <file>

### Undo the last commit but keep changes
git reset --soft HEAD~1

### Undo the last commit and discard changes
git reset --hard HEAD~1
        </code></pre>
    </div>

    <div class="section">
        <h2>9. Tags</h2>
        <pre><code># Create a new tag
git tag <tag_name>

### List all tags
git tag

### Delete a tag
git tag -d <tag_name>

### Push tags to remote

git push origin --tags
        </code></pre>
    </div>

    <div class="section">
        <h2>10. Rebase</h2>
        <pre><code># Rebase the current branch onto another branch
git rebase <branch_name>

### Abort a rebase

git rebase --abort

## 11. Stashing</h2>

### Stash current changes

git stash

### Apply the stashed changes
git stash pop

### List all stashes
git stash list

### Drop a stash

git stash drop

## 12. Other Useful Commands</h2>

### View the change history of a file

git log -- <file>

### View differences between unstaged changes
git diff

### View differences between staged changes and the last commit
git diff --staged

Created by DanhLC - This Git and GitHub Cheat Sheet provides a quick reference to essential commands.
For more advanced usage, refer to the https://git-scm.com/doc Git documentation
