# 명령어 정리

## git init
- 현재 디렉토리에 `.git` 폴더를 생성하여 새로운 git 저장소를 초기화

## git 저장소 만들기 

1) clone : ~에서 복사해오다 (현재 디렉토리에 원격저장소 폴더를 복제)
```
git clone {remote_url}
git clone {remote_url} {directory_name}
```
=> git에 올린내용이 내 컴퓨터로 복제

## `git status`
- 현재의 상태를 확인
    - tracked, untracked 파일을 구분해서 표시

## `git add`
- working directory에서 변경된 파일을 staging area에 이동.

```git add {add_name/directory_name}
git add . => 현재 나의 위치를 기준으로 모든 파일과 폴더
```

## `git commit`
- staging area에 있는 변경사항을 커밋하여 스냅샵 생성

## github에 올리기
- git add .
- git commit
- git esc i (insert 모드)
- update files 
- wq

## 알고 있어야 할 사항

- 터미널 오작동시
    - kill terminal
    - ... 터미널 다시 생성

- git. init -> desttop(master) 표시
    - 데스크탑에 git 위치한다는 뜻
    - rm -r.git (지워져야 함.)

- 되돌리고 싶을때 (메시지 수정)
    - git amend 

## `git log`
- 커밋의 히스토리 조회
    - option 
        - `--oneline`
        - `--graph`

## `git remote`
- 원격저장소 관리 명령어
    - 일반적으로 별명은 `origin` 사용

- 원격 저장소 추가 

```
git remote add {remote_name} {remote_url}
```

- 원격 저장소 확인 
```
git remote -v
```

- 원격 저장소 삭제
```
git remote remove {remote_name}
```