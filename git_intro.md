#   CVCS
    Centralized Version Control systems
#   DVCS
    Distributed Version Control Systems
    
    
#   File's three stages
    1.modified
    2.staged(index)
    3.committed
    
    git file: the files in the VCS
    modified: in the working tree modify git file
    staged: the modified git file store in a stage;
    committed: commit into the repositories;
    
#   Download
    Linux:sudo apt-get install git
    mac : xcode, homebrew,
    
    
#   create repository
    git init
    git clone
    
#   version management
    git add
    git commit 
    git rm

#   check info
    git help
    git log
    git diff
    
#   remote
    git pull
    git push
    
    
#   git committer
    git config --global user.name "Your name"
    git config --global user.email you@example.com
    
#    gitconfig and commands
    
    
    1. /etc/gitconfig       :git config --system
    2. ~/.gitconfig         :git config --global
    3. project, .git/config :git config --local
    
    git config --local user.name ' '
    git config --local --unset user.name
    
    git checkout -- filename :discard change
    
    git reset HEAD test.txt :unstage
    
    git commit --amend -m 'message' :if the message is wrong, then use amend to rewrite the message;

#   vim command and linux command
    control + e: end of line
    control + a: begin of line
    shift + a : end of page
    echo '' > text.txt  :override all content
    
#   git rm vs rm
    git rm:
        git rm test2.txt
        1. delete a file
        2. the deleted file in (stage, index)
        
        -recover back the deleted file
        
        git reset HEAD test2.txt :unstage the deleted file back to working tree
        git checkout --test2.txt :discard the change on the working tree
        
        rm
        using rm the deleted file havent add to stage: can not commit
        rm test2.txt
        git add test2.txt : send to stage;
        

#   git log
    
    -p
    -n
    --stat
    --pretty = oneline
    --pretty = format: "%h-%an,%ar:%s"
    