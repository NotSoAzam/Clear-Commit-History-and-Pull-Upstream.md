# Clear Commit History:
* Remove the history
```
rm -rf .git
```

* Recreate the repos from the current content only
```
git init -b main
git add .
git commit -m "Initial commit"
```
* Push to the github remote repos ensuring you overwrite history
```
git remote add origin git@github.com:revisitable/<repo>.git
git push -u --force origin main
```
# Pull Upstream:
* Fetch Upstream
```
git fetch upstream
```

* Check out main
```
git checkout main
```

* Merge changes
```
git merge upstream/main
```
