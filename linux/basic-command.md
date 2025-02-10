# 리눅스 기본 명령어

## 0. 명령어의 기본형식 
```
command [options] [arguments]
```
- command : 실행할 명령어, 프로그램
- options : 명령어의 옵션
- arguments : 명령어에 전달한 인자, 데이터

## 1. 파일 및 디렉토리 관리

### ls (list)
- list : 디렉토리 내용 목록을 보여줍니다. 
- options : 
    - `-l` : 파일의 상세 정보 표시
    - `-a` : 숨김 파일 표시 (.형식은 숨김 의미)
        - . : 현재 폴더 의미
        - .. : 나보다 상위 폴더

### cd (change directory)
- 현재 작업 디렉토리를 변경합니다. 
- `cd {target-directory}`
- 예시 : cd ~/deskTOP/damf2/TIL

### pwd (print working directory)
- 현재 작업중인 디렉토리의 전체경로를 출력.

### mkdir (make directory)
- 새로운 디렉토리 생성
- `mkdir {directory-name}`

### touch
- 새로운 파일을 생성.
- `touch {file-name}`

### rm (remove)
- 파일이나 폴더를 삭제 
(rm은 폴더는 지울 수 없음 -> 지우기 위해서는 옵션을 넣어야함!)
- options
    - `-r`: recursion (재귀)

### cat (concatenate)
- 파일의 내용을 출력.

### **git init (git inital)**

git 정의 : 어떤 부분을 개선했는지를 보여줌. 변화량을 지속적으로 트래킹함. 
- 0) git init :  한번 하면 이후 할 필요 없음. 

- 1) git add . : 현재 모든 폴더를 추가함.
(이때의 점은 현재 모든 폴더를 의미함.)

- 2) git commit -m "first commit"
(이떄의 m은 메세지를 의미 : 어떤 변화가 생겼는지 적기)

- 3) git config --global user.email or name ""
(누가 하고자 하는지 정의 필요)

### git push origin master
- remote : 원격 저장소 
- push : 올린다
- origin : 별명 