git reset --hard origin/master
- - - 
*sync up master to origin/master*
git branch master
git checkout master
git fetch origin
git reset --hard origin/master
- - - 
git diff --stat 9c77fd5   #commit summary
- - -
*SPLITTING A COMMIT*
- - -
*REBASE!*
git rebase --interactive HEAD~3
 
*RESET COMMIT: undoes the commit and leaves modifies files unstaged:*
git reset HEAD^
 
*ADD ONLY (P)ARTS OF A FILE*
git add -p <filename>
y - (y)es, stage hunk
n - (n)o, don't stage hunk
s - split into smaller hunks
e - manually edit hunk
j - (j)ump to next hunk (going back to this later)
d - go to next file
 - - -
*pull other check-in, but don't commit*
git cherry-pick <shortSHA> -n
- - -
git reset HEAD~                                 #split apart most recent commit
git config --global alias.last 'git -1 HEAD'    #git aliases
git checkout -b foo_bar                         #checkout + switch to branch
- - -
git co master
git merge hotfix
- - -
git br -v
git checkout -b serverfix origin/serverfix
