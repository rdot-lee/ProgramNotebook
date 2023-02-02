### <span style="color:Red"> Init</span>

``` 
git init 
```

### <span style="color:Red"> Branch</span>
```
To rename the current branch:
-git branch -m "NewName"

To rename a branch while pointed to any branch:
-git branch -m "oldname" "newname"

Create New Branch and checkout this
-git checkout -b "Branch"

Checkout Branch
-git checkout "Branch"

```

#### <span style="color:Red"> Remote</span>
```
add:
-git remote add "name" "URL"

rename remote address:
-git remote set-url "name" "NewURL"

rename database name:
-git remote rename "Old" "New"

check URL:
-git remote -v

Delete remove origin:
-git remote remove "origin"
```

#### <span style="color:Red"> Commit</span>
```
git commit -m "message"

git commit ->enter i ->  vim UI -> :wq (save)
```


#### <span style="color:Red"> Push</span>
```
git push -u "name" "URL"
```


#### <span style="color:Red"> Reset</span>
```
Mixed(defulit) : 回到工作目錄
-git reset HEAD~ (HEAD^)

soft : 回到暫存區
-git reset --soft HEAD~

hard : 回到最初
-git reset –hard HEAD~

```
|  Command | Change History  |   |
|  ----    | ----            | ----|
| Reset    | Y          |把目前的狀態設定成某個指定的 Commit 的狀態，通常適用於尚未推出去的 Commit。
| Rebase   | Y          |不管是新增、修改、刪除 Commit 都相當方便，用來整理、編輯還沒有推出去的 Commit 相當方便，但通常也只適用於尚未推出去的 Commit。
| Rever    | N          |新增一個 Commit 來反轉（或說取消）另一個 Commit 的內容，原本的 Commit 依舊還是會保留在歷史紀錄中。雖然會因此而增加 Commit 數，但通常比較適用於已經推出去的 Commit，或是不允許使用 Reset 或 Rebase 之修改歷史紀錄的指令的場合。


#### <span style="color:Red"> Merge</span>
```
example : A merge B
Step 1 : git checkout B
Step 2 : git merge A

```
How to merge when multiple people are working together
http://tech-marsw.logdown.com/blog/2013/08/17/git-notes-github-n-person-cooperation-settings


## Create a Merge Commit

## Squash and Merge

## Rebase and Merge
https://rietta.com/blog/github-merge-types/
