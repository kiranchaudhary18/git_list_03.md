#### Task 1: Create a Local Git Repository

1.first create a folder
```
  mkdir new_folder
  cd new_folder
```
2.intilize a folder
```
  git init
```
3.verify repository status
```
git status
```

#### Task 2: Clone a Remote Repository

1.clone the github repository anyone
```
 git clone 
```

2.check the clone repository status 
```
  cd repo
  ls -a
```

#### Task 3: Commit Changes Locally

1.create a new file
```  
  echo "hi" >file.txt
```

2.add the file  github and commit
```
  git add .
  git commit -m "hello"
```

#### Task 4: Write Effective Commit Messages

1.create a detailed commit message
```
  git commit -m "hi"
```
2.create a multiple file and commit 
```
  touch file2.txt file3.txt
  git add .
  git commit -m "i am kiran"
```

#### Task 5: View Detailed Commit History

1.view full commit history
```
  git log
```
2.view commit history in compact format
```
  git log --oneline
```

####  Task 6: Customize Log Outputs 

1.view logs with a graphical representation
 ```
  git log --oneline --graph --decorate
 ```

 2.filter log for a specific file
```
   git log file1.txt
```

#### Task 7: Understanding Branching

1.check the branch list
 ``` 
  git branch
```
2.create a new branch 
```
  git branch feature
```
3.swicth the branch
```
  git checkout feature
```
#### Task 8: Make Changes in a Branch  

1.create a new file and add the file githu and commit
```
echo "file" >file.txt
git add .
git commit -m "commit"
```

#### Task 9: Merging Branches

1.switch back to the main branch
 ```
 git checkout main
```
2. merge the feature branch in main 
```
  git merge feature
```

#### Task 10: Simulate a Merge Conflict

1.Modify the same line in a file on two branches:
```
echo "Main branch content" > conflict.txt
git add conflict.txt
git commit -m "Added conflict.txt in main branch"
```

2.Switch to the other branch and make conflicting changes:
```
git checkout feature-branch
echo "Feature branch content" > conflict.txt
git add conflict.txt
git commit -m "Modified conflict.txt in feature-branch"
```

3.Merge feature-branch into main:
```
git checkout main
git merge feature-branch
```

4.Resolve the conflict by editing the file and choosing the correct version:
```
    Open conflict.txt and decide which changes to keep.
    Stage the resolved file:

    git add conflict.txt

Commit the merge:

git commit -m "Resolved conflict in conflict.txt"
```

#### Task 11: Delete a Branch

1.delete a branch
```
  git barnch -d feature
```
2.force-delete  branch ( branch hasn`t merged)
```
  git branch -D feature 
``` 

#### Task 12: Rename a Branch

1.rename a current branch
```
 git branch -m main
```
2.rename another branch (not checked out)
```
  git branch -m feature main
```  