### Init

``` git
git init
```

### Branch

```git
To rename the current branch:
-git branch -m "NewName"

To rename a branch while pointed to any branch:
-git branch -m "oldname" "newname"

Create New Branch and checkout this
-git checkout -b "Branch"

Checkout Branch
-git checkout "Branch"

```

#### Remote

```git
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

#### Commit

```git
git commit -m "message"

git commit ->enter i ->  vim UI -> :wq (save)
```

#### Message Type:

- feat: 新增/修改功能 (feature)。
- fix: 修補 bug (bug fix)。
- docs: 文件 (documentation)。
- style: 格式 (不影響程式碼運行的變動 white-space, formatting, missing semi colons, etc)。
- refactor: 重構 (既不是新增功能，也不是修補 bug 的程式碼變動)。
- perf: 改善效能 (A code change that improves performance)。
- test: 增加測試 (when adding missing tests)。
- chore: 建構程序或輔助工具的變動 (maintain)。
- revert: 撤銷回覆先前的 commit 例如：revert: type(scope): subject (回覆版本：xxxx)。



#### Push

``` git
git push -u "origin" "branchName"
```


#### Reset

``` git
Mixed(defulit) : 回到工作目錄
-git reset HEAD~ (HEAD^)

soft : 回到暫存區
-git reset --soft HEAD~

hard : 回到最初
-git reset –hard HEAD~

```

| Command | Change History |                                                                                                                                                                                                                                |
| ------- | -------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Reset   | Y              | 把目前的狀態設定成某個指定的 Commit 的狀態，通常適用於尚未推出去的 Commit。                                                                                                                                                    |
| Rebase  | Y              | 不管是新增、修改、刪除 Commit 都相當方便，用來整理、編輯還沒有推出去的 Commit 相當方便，但通常也只適用於尚未推出去的 Commit。                                                                                                  |
| Rever   | N              | 新增一個 Commit 來反轉（或說取消）另一個 Commit 的內容，原本的 Commit 依舊還是會保留在歷史紀錄中。雖然會因此而增加 Commit 數，但通常比較適用於已經推出去的 Commit，或是不允許使用 Reset 或 Rebase 之修改歷史紀錄的指令的場合。 |

#### Merge

``` text
example : A merge B
Step 1 : git checkout B
Step 2 : git merge A
```

How to merge when multiple people are working together
Ref： <http://tech-marsw.logdown.com/blog/2013/08/17/git-notes-github-n-person-cooperation-settings>

- Create a Merge Commit
- Squash and Merge
- Rebase and Merge
- Ref ： <https://rietta.com/blog/github-merge-types/>



