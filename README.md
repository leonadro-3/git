# git
## 깃 정리 (로컬)

1. 깃을 설치하면 로컬에서 돌아간다.
2. 로컬에서 .git init를 하여 초기 값을 설정한다.
3. git config --global user.name
4. git config --glboal user.email
5. git help tutorial
6. git help log
7. git config --list
8. echo > "example.txt" (q로 탈출)
9. del "파일" (삭제)
10. git status
11. git commit
12. git diff --cached
13. git show (커밋 해쉬값)
14. git reset --hard HEAD^
15. git checkout (커밋 해쉬값)
16. git log
17. git branch
18. git switch "master"

## 깃 정리 (github)

1. 깃허브 사이트에서 만든 레포에서 add 버튼에 있는 URL의 git 주소를 가져온다.
```
https://github.com/leonadro-3/e-shop.git
```

2. 다음 과정을 거친다.  
```
PS C:\Users\82106\Desktop\backend> git remote add origin https://github.com/leonadro-3/e-shop.git
PS C:\Users\82106\Desktop\backend> git remote -v
origin  https://github.com/leonadro-3/e-shop.git (fetch)
origin  https://github.com/leonadro-3/e-shop.git (push)
PS C:\Users\82106\Desktop\backend> git branch
* master
PS C:\Users\82106\Desktop\backend> git push origin master
Enumerating objects: 993, done.
Counting objects: 100% (993/993), done.
Delta compression using up to 16 threads
Compressing objects: 100% (939/939), done.
Writing objects: 100% (993/993), 1013.77 KiB | 1.62 MiB/s, done.
Total 993 (delta 157), reused 0 (delta 0), pack-reused 0 (from 0)     
remote: Resolving deltas: 100% (157/157), done.
remote:
remote: Create a pull request for 'master' on GitHub by visiting:     
remote:      https://github.com/leonadro-3/e-shop/pull/new/master     
remote:
To https://github.com/leonadro-3/e-shop.git
 * [new branch]      master -> master
PS C:\Users\82106\Desktop\backend> 
```

3. 자동으로 main과 master 브런치가 분리되어 업로드 된다.


## 깃 오류

```
PS C:\Users\82106\Desktop\backend> git push orgin master
fatal: 'orgin' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
PS C:\Users\82106\Desktop\backend> 
```

로컬에서 작업한 것들을 깃허브로 업로드하기 위해 push를 했지만 오류가 뜬다.  

```
PS C:\Users\82106\Desktop\backend> git push origin master
```

철자가 틀렸다.  

