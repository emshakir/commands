`How to check for changes on remote (origin) Git repository`
```text
Step 1:
git fetch origin

Step 2:
git checkout -b localTempOfOriginMaster origin/master // moving to new branch in local
git difftool HEAD~3 HEAD~2
git difftool HEAD~2 HEAD~1
git difftool HEAD~1 HEAD~0
Step 3:

git checkout master
git branch -D localTempOfOriginMaster
git merge origin/master
```

`Add an existing project to GitHub steps`
```markdown
git init
git add .
git status
git commit -m "message"
git remote add origin https://github.com/[username]/[repository-name].git
git remote -v
git push -u -f origin/[branch-name]
    -u: switch makes the remote GitHub repo the default for your existing project.
    -f: switch forces Git to overwrite any files that already exist on GitHub with your existing project’s files.
```
