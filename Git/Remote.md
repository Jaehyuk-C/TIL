# 원격저장소

## 원격저장소 조회

```bash
$ git remote -v    # verbose
```

```bash
origin  https://github.com/Jaehyuk-C/test.git (fetch)
origin  https://github.com/Jaehyuk-C/test.git (push)
```



## 원격저장소 추가

```bash
$ git remote add origin <원격저장소이름> <주소>
```

- 깃아, 원격저장소(`remote`)를 추가해줘 (`add`). `origin` 이라는 이름으로, `주소`를



## 원격저장소 삭제

```
$ git remote rm <원격저장소이름>
```



## 원격저장소 push

```bash
$ git push <원격저장소이름> <브랜치 이름>
$ git push origin master
```

## 원격저장소 clone

```bash
$ git clone <원격저장소이름>
```



