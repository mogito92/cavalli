# Git setup & merge commands (PowerShell)

Use these copy/paste commands to set your Git identity and re-run the merge on the PR branch.

```powershell
git config --global user.name "Mogito92"
git config --global user.email "filiseve@gmail.com"

git merge origin/main
```

If the merge reports conflicts:

```powershell
git status -sb
```

Resolve the conflict markers in `index.html`, then:

```powershell
git add index.html
git commit -m "Resolve merge conflicts in index.html"
git push origin codex/locate-index-mfcugn
```
