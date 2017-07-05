https://yxxxxxi@github.com/ynozaki/myMachineLearning.git
To see options, enter ’command’ -h

##Some useful commands
#Set up
$git remote origin “URL”
$git remote set-url origin “new URL”
$git config —global user.name “”
$git config —global user.email xx@xx.xx

#Add
$git add “file” 
(Or git add ., or git add -A)
If you wish to exclude useless files, like .DS_Store, do
$git config —global core.excludesfile $HOME/.gitexclude
$echo “.DS_Store” >> $HOME/.gitexclude
(Or project/.gitignore abc,!abc,*.abc,*.[abc],abc/,abc)

#Commit
$git commit -m “comment” 
(or type $git commit -a -m “comment”, if the file already exists in the index)
To overwrite the lated commit
$git commit —amend

#Push
$git push origin master

#Discard all changes, back to the latest commit
$git reset —hard HEAD 
(Here, “HEAD” means the latest commit ID. HEAD~ means the one just before the latest ver)
Or, only specified file(s),
$git checkout HEAD “file”

#Revert
$git reset —hard HEAD (if need)
$git revert “commit ID”

#Rebase
$git reset —hard HEAD^
$git rebase -i “commit ID”
After rebasement, do
$git rebase —amend
And to resume, do
$git rebase -continue

#Remove
$git rm “file”
If you wish to remove only from index, do
$git rm —cached “file”
Then the file remains in your working space.

#Rename
$git mv “before” “after”

#Unstage
$git reset HEAD “file”

#Clone
$git clone “Path to the folder to be cloned” “folder to be created”

#Pull
$git pull “Path to the folder to be pulled”

#Show
$git show (to see the latest commit ID)
$git statue (to see On branch master)
$git log
$git log —oneline
$git diff “old” “new”


