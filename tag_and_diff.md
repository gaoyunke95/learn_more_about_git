# Tag And Diff

### Tag
    two types:
            1.lightweight
            2.annotated
            
    LIGHTWEIGHT
        git tag v1.0.1
        
    ANNOTATED
        git tag -a v1.0.2 -m 'release version'
        
    DELETE tag
        git tag -d tag_name
        
    git tag: list out all the tag
    git tag -l 'v*'
    
### diff
    show the difference of files;
    
    diff -u a b
    "-"sign: the resource file
    "+"sign: the target file
    @@-1,3 +1,3@@ (- source file 1 firstline 3 last line; + target file)
    
###### git diff
    git diff : show difference between working and stage
    
    git diff 
    "-" in the stage 
    "+" in the working 
    
    
    git diff HEAD: show difference between working and the most recent committed
    
    git diff --cahed commit_id
    
    git diff --cahed: show difference between stage and most recent committed
    

### blame
    Show what revision and author lastmodified each line of a file
    
    git blame filename