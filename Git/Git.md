### <span style="color:Red"> Init</span>
git init 


### <span style="color:Red"> Branch</span>
##### To rename the current branch:
git branch -m "NewName"
##### To rename a branch while pointed to any branch:
git branch -m "oldname" "newname"
##### Create New Branch and checkout this
git checkout -b "Branch"
##### Checkout Branch
git checkout "Branch"

#### <span style="color:Red"> Remote</span>
##### add:
git remote add "name" "URL"
##### rename remote address:
git remote set-url "name" "NewURL"
##### rename database name:
git remote rename "Old" "New"
##### check URL:
git remote -v
##### Delete remove origin:
git remote remove "origin"

#### <span style="color:Red"> Commit</span>
git commit -m "message"

git commit ->enter i ->  vim UI -> :wq (save)

#### <span style="color:Red"> Push</span>
git push -u "name" "URL"

#### <span style="color:Red"> Reset</span>
##### Mixed(defulit) : 回到工作目錄
git reset HEAD~ (HEAD^)
##### soft : 回到暫存區
git reset --soft HEAD~
##### hard : 回到最初
git reset –hard HEAD~

#### <span style="color:Red"> Merge</span>
example : A merge B
Step 1 : git checkout B
Step 2 : git merge A

##### How to merge when multiple people are working together 
http://tech-marsw.logdown.com/blog/2013/08/17/git-notes-github-n-person-cooperation-settings