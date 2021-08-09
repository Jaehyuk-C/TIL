# Git 특강

## 1. init

```bash
$ git init
```

- 현재 경로의 폴더를 git 저장소로 만들어 git으로 관리
  - git 폴더가 생성되며
  - git bash에서는 (master)라는 표기를 확인할 수 있음

![이미지1](C:\Users\Jaehyuk Choi\Desktop\BIG DATA\md-image\캡처.PNG)

## 2. add

#### add . VS add <파일명>

- 수정이 동시에 일어나는 파일들이라면 'add .' 으로  묶어서 staging area에 올리기

```bash
$ git add .
```



- 수정이 따로 일어나는 파일들이라면 'add <파일명>'을 통해 따로 staging area에 올리기

```bash
$ git add <filename>
```





## 3. commit

```bash
$ git commit -m"commit mesege"
```

- 앞서 add 를 통해 staged 된 파일들을 커밋을 통해 버전으로 기록
- 변경사항이 무엇인지 알 수 있게 커밋메세지를 명확히 작성



## 4. status

```bash
$ git status
```

- Git 저장소에 있는 파일의 상태를 확인하기 위하여 활용

  - 파일의 상태를 알 수 있음 
    - Untracked files 
    - Changes not staged for commit 
    - Changes to be committed

  - Noting to commit, working tree clean

![캡처1](C:\Users\Jaehyuk Choi\Desktop\BIG DATA\md-image\캡처1.PNG)



## 5. log

```bash
$ git log
```

- 현재 저장소에 기록된 커밋을 조회

- 다양한 옵션을 통해 로그를 조회할 수 있음 

  ```bash
  $ git log -1 
  $ git log -oneline 
  $ git log -2 --oneline
  ```

  

## 6. config

- —system
  - /etc/gitconfig 
  - 시스템의 모든 사용자와 모든 저장소에 적용(관리자 권한)
- —global
  - ~/.gitconfig
  - 현재 사용자에게 적용되는 설정
- —local
  - .git/config
  - 특정 저장소에만 적용되는 설

