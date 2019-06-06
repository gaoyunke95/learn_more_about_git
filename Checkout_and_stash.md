# Checkout And Stash
    
    git checkout -- filename
    discard the changes on working tree; the last change before stage;
    
    git reset HEAD -- filename
    
    
    git stash (save the change of the branch for use of later)
    
    git stash list(show the list of stash)
    
    git stash save 'message'
    
    git stash pop (take out the status delete the status on the list)
    
    git stash apply (take out the status but not delete)
    
    git stash apply stash@{0}
    
    git stash drop stash@{1} (delete the status)