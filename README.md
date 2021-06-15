# git-laboraotry

### git 작업
1. issue 생성(github > Issues > Nnew issue)
2. issue 에 맞는 브랜치 생성
```shell
$ git checkout -b feature/wordbe/#1-write-todo
# checkout -b 는 branch 로 새로운 브랜치를 만들고, checkout으로 해당 브랜치에 체크아웃한다.
```

코드를 수정한 후
```shell
# Working Directory -> Staging Area
$ git add [수정한 파일]

# Staging Area -> Repository
$ git commit -m "feat: 할일 입력"

# Respository -> 원격저장소
$ git push # 실패
# 브랜치를 새로 생성한 후에는 푸쉬할 원격저장소와 이어주어야 함
# 다음부터는 바로 push 해도 됨
$ git push --set-upstream origin feature/wordbe/#1-write-todo
```

3. pull request 작성
4. review 요청
5. merge
