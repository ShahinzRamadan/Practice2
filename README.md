# practice branching and merging
  ### creating new branch:-
    git branch BranchName
  ### switch to a branch:-
    git checkout BranchName
  ### creating a new branch and switching to it at once:-
    git checkout -b BranchName
  ### rename a branch:-
    git branch -m NewName
  ### merging with master:-
    git merge BranchName
  ### pushing the new branch:-
    git push origin BranchName
  ### deleting a branch:-
    git branch -d BranchName
    git branch -D BranchName


# practice stash command
  ### stash files in the staging area:-
    git stash
  ### stash a file with a message:-
    git stash save "message"
  ### list the existing stashes:-
    git stash list
  ### show the contents of the latest stash:-
    git stash show
  ### show the contents of a specific stash:-
    git stash show stash@{id}
  ### get the files out of the latest stash and drop the stash:-
    git stash pop
  ### get the files out of the latest stash without dropping the stash:-
    git stash apply
  ### get the files out of a specific stash:-
    git stash pop/apply stash@{id}
  ### drop the latest stash(and its contents):-
    git stash drop
  ### drop a specific stash:-
    git stash drop stash@{id}
  ### drop all the stashes:-
    git stash clear
  ### pop the files out from the stash in a new branch:-
    git stash branch BranchName

  
 
