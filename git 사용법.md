# Git

##기본명령어

1.git 저장소 (repository) 초기화
```bash
$ git init
```

원하는 폴더를 저장소로 만들게 됨 `git bash` 에서 (`master`) 표기됨

숨김폴더로 `.git/` 폴더가 생성됨



2.커밋할 목록에 담기 (`staging area`)

```
$ git add . 
```
현재 작업공간(`Working Directory/Tree`)의 변경사항을
커밋할 목록에 추가한다(`add`)

(` .  `)은 리눅스에서 현재 디렉토리(폴더)를 표기하는 방법으로 
현재 내 폴더에 있는 파일의 변경사항을 전부 추가한다

단일 파일만 추가하려면 `git add "파일이름"`

폴더를 추가하려면 `git add "폴더이름"` 

3 커밋하기
```
$ git commit -m '_______' 
```
커밋을 할때에는 해당하는 버전의 이력을 의미하는 메세지를 
반드시 적어준다 `-m`

메세지는 지금 버전을 쉽게 이해할 수 있도록 작성한다

커밋은 현재 코드의 상태를 스냅샷 찍는 것이다.

4 git log 기록 확인하기

5 git status 상태 확인하기

CLI(Command Line Interface) 현재 상태를 알기 위해 반드시
명어를 통해 확인한다

커밋할 목록에 담겨 있는지, untracked 인지, 커밋할 내역이 
있는지 등등 다양한 정보를 알려준다. 





# 원격저장소 활용하기



1. 원격저장소 (remote repository) 등록하기

```bash
$ git remote add ___이름____ _____경로-____
```

​	원격 저장소(remote) 를 등록(add) 한다. origin 이름으로 경로를 

​	최초로 한번만 등록하면 된다

​	아래의 명령어로 현재 등록된 원격 저장소를 확인할 수 있다



```bash
$ git remote --v 
origin  https://github.com/sjagz/first20190524.git (fetch)
origin  https://github.com/sjagz/first20190524.git (push)

```



2. 원격 저장소에 올리기 (push)

```bash
$ git push origin master
```

​	git에 올리기(push) 이름 (origin )인 것을 원격저장소에 master 로



3. 원격 저장소로부터 가져오기(pull)

```bash
$ git pull origin master
```

# 원격저장소 복제(clone) 하기

```bash
$ git clone ____경로____
```

깃배쉬에서 원하는 폴더 경로를 찍어주고

경로는 깃허브 레파지토리에서 우측  clone or download 클릭해서 링크(경로)



