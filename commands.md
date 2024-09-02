Git-Task-1 Commands

1. fork: creates a copy of a repository on your own git account
   clone: creates a copy of a repository on you local machine

2. touch "Amitesh Singh.txt"   :touch is used to create an empty file
                                unless you "add" the file the tree will not reflect it, upon adding the tree structure for next file will reflect this
                                and if you later commit it the git tree object for that commit will include the new file
   git add "Amitesh Singh.txt"  :git add bsically tells Git that you want to include updates to a particular file in the index for the next commit
                                 it itself does not modify the Git tree
   git commit -m "Initial commit"  :a commit records snapshots of all tracked files in the directory, bascially copy and paste
                                    commit updates the tree object to reflect the changes, commit also records the previous commit as its parent
                                    which creates a chain of commits which helps in tracking the history of changes

3. git branch Amitesh  :git branch creates a new branch in local repository
                        branches are pointers to a specific commit and updates working directory to reflect state of that commit, it doen't directly modify the tree
                           
4. git checkout Amitesh  :checkout is used to switch branches
                          tree is not modified
   touch AmiteshSing.md  : touch is used to create an empty file
                           unless you "add" the file the tree will not reflect it, upon adding the tree structure for next file will reflect this
                           and if you later commit it the git tree object for that commit will include the new file

5. git log  :shows commit history where you can see the commit hash
             does not make changes to the tree
   nano AmiteshSingh.md  :nano is a text editor
                          it does not change the tree
   git add AmiteshSingh.md  :git add basically tells Git that you want to include updates to a particular file in the index for the next commit
                             it itself does not modify the Git tree
   git commit -m "Added commit hash of last commit"  :a commit records snapshots of all tracked files in the directory, bascially
                                                                        copy and paste
                                                                        commit updates the tree object to reflect the changes, commit also records the previous commit as its parent
                                                                        which creates a chain of commits which helps in tracking the history of changes

6. git checkout main  :checkout is used to switch branches
                     tree is not modified
   git merge Amitesh  :merge combines from one or more branch into current branch
                       the merge commit includes a new tree object that represents the combined state of the files from both the branches 

7. nano README.md  :nano is a text editor
                    it does not change the tree
   git add README.md  :git add basically tells Git that you want to include updates to a particular file in the index for the next commit
                       it itself does not change the tree
   git commit -m "Added my name"  :a commit records snapshots of all tracked files in the directory, bascially copy and paste
                                              commit updates the tree object to reflect the changes, commit also records the previous commit as its parent
                                              which creates a chain of commits which helps in tracking the history of changes
   git reset --soft HEAD^  :reset reverses changes by moving a branch reference backwards to an older commit, its like rewriting history
                            soft is so that the changed files are "changes to be commited"
                            HEAD is the symbolic name for the currently checked out commit, basically points to the most recent commit
                            ^ is a relative ref which moves upwards one commit at a time
   git restore --staged README.md  :it is used to unstage
                                    no changes made to the tree

8. nano commands.md  :nano is a text editor and creates commands.md
                      it does not change the tree
   git add commands.md  :git add basically tells Git that you want to include updates to a particular file in the index for the next commit
                         it itself does not change the tree
   git commit -m "Added commands used throughout the task"  :a commit records snapshots of all tracked files in the directory, bascially copy and paste
                                                             commit updates the tree object to reflect the changes, commit also records the previous commit as its parent
                                                             which creates a chain of commits which helps in tracking the history of changes

9. git push origin main  :allows us to transfer files from local repository(origin) to remote directory(main)
   git pull origin main  :allows us to fetch and integrate changes which are present in remote repository to the local repository
   
