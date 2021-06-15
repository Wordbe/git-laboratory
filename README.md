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
github 의 해당 저장소에 들어가면, 위에 노란 배너와 초록색 버튼에 Compare & pull request 가 생긴다.

내용에 close #1 을 입력하면,
pull requests 가 merge 될 때 이슈도 같이 close 된다.


4. review 요청
리뷰어를 선정하고 리뷰를 받는다.
(수정할 것이 있다면) 코드를 수정하고, commit 한다.

5. merge
