1.'git init' -> powers your folder to be managed by git, and initializes a new empty repository.It also creates a new .git folder that has all the relevant logic to manage versions of your project.

2.'working area' -> There can be a bunch of files that are not currently handled by git.It means that changes done in those files are not managed by git yet.A file which is in working area is considered to be not in the staging area. When we do 'git status' and we see a bunch if 'untracked files' then these are actually called to be in the working area.

3.'Staging Area' -> what all files are going to be part of the next version that we will create.This staging area is the place git knows what changes will be done from the last version to the next version.

4.'Repository Area' -> This area actually contains the details of all the previous registered version.And the files in this area, git already manages them and knows there version history.

5. 'git add <file>' -> moves file from working area to staging area.

6. 'git rm --cached<file>' -> moves files back from staging area to working area.

7. 'commit' -> Commit is a particular version of the project.It captures a snapshot of the projects's staged changes and creates a version out of it.

8. 'git commit' -> registers staging changes to a commit.

9. 'git log' -> list downs all the commits of the repository.Press 'q' to exit out of the git log.

10. 'git restore <file>' -> it removes all files chnages from the staging area to be committed.This can be useful, if we did some dirty piece of code and now no more want it.Instead of deleting every change line by line, we can restore it or you can restore last clean version of the file/ last commit.

11. 'git restore --staged <file>' ->It removes file from changes from staging area to wor king area.
this is the bad code.

 12. Diff b/w git rm and git restore
 ans: -> if you want the whole file back to the untracked state i.e in the working area , then we do git rm, otherwise if we just want changes to be moved in the working area or staging area then we get restore.

13. 'git diff commit1 commit2' -> gives the differnce of all file changes between two commits.

14. 'git commit -m "your commit message"' -> if you want to avoid opening a text editor like vim/nano to add a commit message use this command.

15. 'git remote' -> list down all the remote connections name.

16. Remote connection  -> It helps to link two git repositories for uploading and downloading changes from each other.

17. 'git remote add <name of remote> <link of the remote>' : this command hepls s to add a new link to the remote repo and give a name to it.

18. 'git remote rm <name of remote>' : this command deletes a remote connection.

19. 'git remote rename <oldname> <newname>' : this command renames the remote connection.

NOTE: The name of the remote connection is always used to establish communication between the repos.

20. 'git add <file1> <file2> <file3>' : this command will add multiple file changes together to the staging area

21. 'git add .' : this command to add all files from working area to staging area.

22. 'git pull <remote name> <branch>' : downloads latest changes from the branch of the mentioned remote to your local repository.

23. ## Recommeded practice to do
  -make changes.
  -git add <file>.
  -git commit.
  -git pull.
  -git push.