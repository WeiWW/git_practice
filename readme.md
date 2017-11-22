#Git Notes
1. `git add *.html` -> add all the html file to staging area
2. `git add --all `-> add all the changes in this project to staging area
3. `git add .`-> add all the changes of cuurent folder to staging area 
4. `git commit -a -m "commit message" `-> add & commit, the files must be tracked file
5. `git log --oneline --graph`
6. `git log --author="author name A\| author name B"`
7. `git log --grep="keyWords"` -> search "key words" in commit messages
8. `git log -S "KEY_WORDS"` -> search all the files in commits has "KEY_WORDS"
9. `git log  --since="9am" --until="12am" --after="2017-01"`
10. `git rm file --cached` -> Don't wanna file be tracked
11. `git mv fileA fileB`-> rename fileA to fileB
12. `git commit --amend -m "new message"` -> change the last commmit message to "new message"(if don't have -m ,will get into Vim model)
13. `git add newFile && git commmit --amend --no-edit` -> add file to last commit and not edit commit message(--no-edit)
14. `mkdir folder && touch folder/.keep && git add`  -> add new folder
15. `git clean -fX` -> forced clean all ignore files
16. `git log filename` -> all logs of this file
17. `git log -p filename` -> all logs and changes of this file
18. `git blame filename` -> list who write each columes in this file.
19. `git blame -L 5,10 filename` -> only show colume No.5~No.10
20. `git checkout filename` -> restore file
21. `git checkout .` -> restore all
22. `git reset SHA-1` -> back to this commit
23. 模式|Commit 拆出來的檔案
------------ | ------------- 
mixed 模式（預設)|丟回工作目錄
  soft 模式|丟回暫存區
  hard 模式|直接丟掉
                       
24. `git reflog == git log -g` -> HEAD moveing record
25. `git branch b1` -> new branch b1
26. `git branch -m b1 B` -> rename branch b1 to B
27. `git branch -d B` -> delete branch B (-D, force delete)
28. `git checkout B` -> change to branch B
29. `git chckout -b C` -> change to branch C, if not exisit branch C, will new a branch C
30. `git merge C -no--ff` -> merge branch C without fast-forward
31. `git reset SHA-before-rebase -hard` -> go back to rebase status
32. `git branch bird SHA = git checkout -b bird SHA` -> new a branch bird on certain commit
33. [**one commit to multi-commit**](http://gitbook.tw/chapters/rewrite-history/split-one-commit-to-many-commits.html)
34. [**between commits add new commit**](http://gitbook.tw/chapters/rewrite-history/add-new-commit.html)
35. [**revert**](http://gitbook.tw/chapters/rewrite-history/reset-revert-and-rebase.html)
36. [**statch**](http://gitbook.tw/chapters/faq/stash.html)
37. [**remove sensitive data - filter-branch**](http://gitbook.tw/chapters/faq/remove-sensitive-data.html)
38. `git cherry-pick 6a498ec --no-commit` -> pick commit and put into stagching area
39. [**really remove file from git**](http://gitbook.tw/chapters/faq/remove-files-from-git.html)

**detached HEAD**

ref: [http://gitbook.tw](http://gitbook.tw)


