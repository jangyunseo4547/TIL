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