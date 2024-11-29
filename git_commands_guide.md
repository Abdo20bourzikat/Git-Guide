// Initialize a Git repository
git init

// Show the status of your code
git status

// Track a single file
git add file.ext

// Commit changes with a message
git commit -m "Your commit message"

// Track changes and commit
git add file.ext  # Stage the file
git commit -m "Your commit message"  # Commit the changes

// Track all files in the directory
git add .

// Show the commit history
git log

// Restore a deleted file or checkout a specific commit
git checkout <commit-hash>  # Replace <commit-hash> with the actual hash

// Ignore a file (stop tracking it)
git rm --cached file.ext  # Untrack the file but keep it locally
// Add the file to .gitignore to prevent future tracking
echo "file.ext" >> .gitignore
// Example to ignore all .php files
echo "*.php" >> .gitignore

// Steps to push your project to GitHub:
// 1. Add the repository URL as a remote named 'origin'
git remote add origin https://github.com/abdo20bourzikat/reponame

// 2. Rename the branch from master to main (if necessary)
git branch -M main

// 3. Push your code to GitHub
git push -u origin main

// Show all remotes
git remote -v

// Create a new branch
git branch branchname

// Delete a branch
git branch -d branchname

// Merge another branch into the current branch (must be on the main branch)
git merge otherBranchName
// Resolve conflicts if any and commit the changes
