# GitScript
Script Git for clone subdirectories

## Run de following comands (Powershell 7.^ or Bash)

### Create dir and change to the created dir
```ps1 
mkdir <folder_xyz> && cd <folder_xyz>
```
### Initiate Git.
```ps1 
git init 
```
### Track the repository with the original github link as if you were cloning
```ps1 
git remote add -f origin <github-link.git>
```
### Enable the tree scanning feature.
```ps1 
git config core.sparseCheckout true
```
### Enter only the subdirectory inside ' '.
```ps1 
echo '<subdir>' >> .git/info/sparse-checkout
```
### Download with Pull and not with Clone (Note the right branch of the repository!)
```ps1 
git pull origin main
```
