# cs_study

**최초 설정**

1. 프로젝트 레포 fork 해서 자신의 github로 복사
2. fork한 프로젝트 자신의 로컬 저장소에 clone
3. 브랜치 생성
   ```
   $ git remote add upstream <원래 프로젝트 레포의 url>
   $ git remote -v
   $ git checkout -b 브랜치이름
   ```

Read Me 생성 혹은 변경 후,

```
$ git add .
$ git commit -m "msg"
$ git push origin 브랜치이름
```

Compare & pull request

Merge 된 후, main 브랜치로 이동하여 upstream의 커밋 내역을 가져와서 동기화

```
$ git checkout main
$ git fetch upstream main
$ git rebase upstream/main
```

로컬에서 동기화 된 이후, 각자의 github에 업로드

```
$ git add .
$ git commit -m "msg"
$ git push
```
