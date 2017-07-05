https://yxxxxxi@github.com/ynozaki/myMachineLearning.git
To see options, enter ’command’ -h

##Some useful commands
#Set up
git remote origin “URL”
git remote set-url origin “new URL”
git config —global user.name “”
git config —global user.email xx@xx.xx

#Push
git add “file” 
(or git add ., or git add -A)
git commit -m “comment” 
(or type $git commit -a -m “comment”, if the file already exists in the index)
git push origin master

#Discard all changes, back to the latest commit
git reset —hard HEAD 
(Here, “HEAD” means the latest commit ID. HEAD~ means the one just before the latest ver)

#or, only specified file(s)
git checkout HEAD “file”

#Remove
git rm “file to be deleted”

#Rename
git mv “before” “after”

#Unstage
git reset HEAD “file”

#Show
git show (to see the latest commit ID)
git statue (to see On branch master)
git log
git log —oneline

#Overwrite the lated commit
git commit —amend

