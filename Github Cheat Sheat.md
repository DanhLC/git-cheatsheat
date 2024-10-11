<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Git and GitHub Cheat Sheet">
    <title>Git and GitHub Cheat Sheet</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            margin: 0;
            padding: 20px;
        }

        h1, h2 {
            color: #333;
        }

        h1 {
            font-size: 2.5em;
        }

        h2 {
            font-size: 1.8em;
            margin-top: 20px;
        }

        pre {
            background-color: #f4f4f4;
            border-left: 5px solid #333;
            padding: 10px;
            font-size: 1em;
            overflow-x: auto;
            white-space: pre-wrap;
            word-wrap: break-word;
        }

        code {
            font-family: "Courier New", Courier, monospace;
            color: #333;
        }

        .section {
            margin-bottom: 40px;
        }

        .section:nth-child(even) {
            background-color: #e9ecef;
            padding: 20px;
        }

        hr {
            margin: 30px 0;
            border: none;
            border-bottom: 2px solid #ccc;
        }

        .note {
            background-color: #fff3cd;
            padding: 15px;
            border-left: 5px solid #856404;
        }

        ul {
            padding-left: 20px;
        }

        ul li {
            line-height: 1.6;
        }

        footer {
            margin-top: 50px;
            text-align: center;
            font-size: 0.9em;
            color: #777;
        }
    </style>
</head>
<body>

    <h1>Git and GitHub Cheat Sheet</h1>

    <div class="note">
        <p>This cheat sheet includes commonly used Git and GitHub commands to help you manage and work with repositories effectively.</p>
    </div>

    <hr>

    <div class="section">
        <h2>1. Set Up and Configure Git</h2>
        <pre><code>
# Set username
<pre><code>git config --global user.name "Your Name"

# Set email
git config --global user.email "youremail@example.com"

# Check configuration
git config --list
        </code></pre>
    </div>

    <div class="section">
        <h2>2. Create and Manage Repositories</h2>
        <pre><code># Initialize a new repository
git init

# Clone a repository from GitHub
git clone https://github.com/user/repository.git
        </code></pre>
    </div>

    <div class="section">
        <h2>3. Status and Information</h2>
        <pre><code># Check the status of your repository
git status

# View commit history
git log

# View a short log history
git log --oneline
        </code></pre>
    </div>

    <div class="section">
        <h2>4. Working with Files</h2>
        <pre><code># Add new or modified files to staging area
git add <file>

# Add all files to staging area
git add .

# Remove a file from staging area
git reset <file>

# Delete a file from both working directory and staging area
git rm <file>

# Move or rename a file
git mv <old_filename> <new_filename>
        </code></pre>
    </div>

    <div class="section">
        <h2>5. Commit Changes</h2>
        <pre><code># Create a commit with a message
git commit -m "Commit message"

# Commit and include unstaged changes
git commit -a -m "Commit message"
        </code></pre>
    </div>

    <div class="section">
        <h2>6. Branching</h2>
        <pre><code># Create a new branch
git branch <branch_name>

# List branches
git branch

# Switch branches
git checkout <branch_name>

# Create and switch to a new branch
git checkout -b <branch_name>

# Merge a branch into the current branch
git merge <branch_name>

# Delete a branch
git branch -d <branch_name>
        </code></pre>
    </div>

    <div class="section">
        <h2>7. Remote Operations</h2>
        <pre><code># List remotes
git remote -v

# Add a new remote
git remote add origin https://github.com/user/repository.git

# Remove a remote
git remote remove <remote_name>

# Fetch changes from remote without merging
git fetch origin

# Pull changes from remote and merge
git pull origin <branch_name>

# Push changes to remote
git push origin <branch_name>
        </code></pre>
    </div>

    <div class="section">
        <h2>8. Undoing Changes</h2>
        <pre><code># Revert file to the last commit
git checkout -- <file>

# Undo the last commit but keep changes
git reset --soft HEAD~1

# Undo the last commit and discard changes
git reset --hard HEAD~1
        </code></pre>
    </div>

    <div class="section">
        <h2>9. Tags</h2>
        <pre><code># Create a new tag
git tag <tag_name>

# List all tags
git tag

# Delete a tag
git tag -d <tag_name>

# Push tags to remote
git push origin --tags
        </code></pre>
    </div>

    <div class="section">
        <h2>10. Rebase</h2>
        <pre><code># Rebase the current branch onto another branch
git rebase <branch_name>

# Abort a rebase
git rebase --abort
        </code></pre>
    </div>

    <div class="section">
        <h2>11. Stashing</h2>
        <pre><code># Stash current changes
git stash

# Apply the stashed changes
git stash pop

# List all stashes
git stash list

# Drop a stash
git stash drop
        </code></pre>
    </div>

    <div class="section">
        <h2>12. Other Useful Commands</h2>
        <pre><code># View the change history of a file
git log -- <file>

# View differences between unstaged changes
git diff

# View differences between staged changes and the last commit
git diff --staged
        </code></pre>
    </div>

    <footer>
        <p>Created by [Your Name] - This Git and GitHub Cheat Sheet provides a quick reference to essential commands.</p>
        <p>For more advanced usage, refer to the <a href="https://git-scm.com/doc" target="_blank">Git documentation</a>.</p>
    </footer>

</body>
</html>
