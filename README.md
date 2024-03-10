# ▶️Practice branching and merging
  ### Creating new branch:-
    git branch BranchName
  ### Switch to a branch:-
    git checkout BranchName
  ### Creating a new branch and switching to it at once:-
    git checkout -b BranchName
  ### Rename a branch:-
    git branch -m NewName
  ### Merging with master:-
    git merge BranchName
  ### Pushing the new branch:-
    git push origin BranchName
  ### Deleting a branch:-
    git branch -d BranchName
    git branch -D BranchName


# ▶️Practice stash command
  ### Stash files:-
    git stash
  ### Stash a file with a message:-
    git stash save "message"
  ### List the existing stashes:-
    git stash list
  ### Show the contents of the latest stash:-
    git stash show
  ### Show the contents of a specific stash:-
    git stash show stash@{id}
  ### Get the files out of the latest stash and drop the stash:-
    git stash pop
  ### Get the files out of the latest stash without dropping the stash:-
    git stash apply
  ### Get the files out of a specific stash:-
    git stash pop/apply stash@{id}
  ### Drop the latest stash(and its contents):-
    git stash drop
  ### Drop a specific stash:-
    git stash drop stash@{id}
  ### Drop all the stashes:-
    git stash clear
  ### Pop the files out from the stash in a new branch:-
    git stash branch BranchName

# 📑Notes
 ### about branch
  * you can't delete a branch while you're switched to it, you have to switch to another branch to delete the other one
  * *git branch -d BranchName* this command checks the branch you are trying to delete first and if it finds out that there are modifications that you didn't merge into the master branch it will refuse to delete it
  * *git branch -D BranchName* this command deletes the branch anyway
  * you have to switch to the master to merge a branch within 
### about stash
 * you will notice a pattern within the stash commands which is if you just write the command this means the command will work on the latest stash you've created, but if you need to work on a specific stash you need to explicitly write the stash id
 * *git stash branch BranchName* this command does several things:-
                                                                   1. create a new branch
                                                                   2. pop the files from the stash to the new branch
                                                                   3. switch to the new branch   
        
 
