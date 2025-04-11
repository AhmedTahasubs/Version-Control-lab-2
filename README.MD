To remove branches locally 
git branch -d branchName          //Safe delete, checks for unmerged changes
git branch -D branchName          //Force delete, ignores unmerged changes

To remove branches remotely  
git push origin --delete branch_name 

And to cleanup the reference to the branch in my local repo after deleting it remotely to keep sync with the remote
git fetch --prune
