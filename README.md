# README

TIL(Todat I Learned)
오늘 배운 내용을 기록합니다. 

- linux
- markdown

- 파랑색 표시 : 폴더 
- ctrol l : 내역 삭제 
- 위 화살표 : 히스토리 볼수 있음.

### 2/11 (월)

### 1. 끝말잇기
```
- git init (한번만 하면 됨)
- git add . (working directory -> staging area로 이동)
- git commit -m "update" (변경된 사항 기록)
- git push origign master (git 레퍼러지로 이동)

- git pull origign master (다른 사람것 불러오기)
```

### 2. 웹사이트 만들기
```
1) 스타트 부트 스트랩에서 원하는 템플릿 다운로드
2) 다운로드 파일 -> 새 폴더 만들고, 다운로드 파일 옮기기 
3) new 레파지토리 만들기 (새로운 이름)
```
**코드**
```
git init (한번만 하면 됨)
git add . (working directory -> staging area로 이동)
git commit -m "update" (변경된 사항 기록)

origin 정의 : git remote add origin https://github.com/jangyunseo4547/jysjys4547.github.io.git)

git push origign master (git 레퍼러지로 이동)

5) add. -> commit -m"update" -> git push (변경사항있을때마다)
```

### 2/12 (화)

## 브랜치

- 나눠서 안정성있게 개발하고 하나로 합쳐지는 과정
```
1) master -> testing 가지치기 : git branch testing

2) 브랜치 이동하기 : git checkout or git switch

3) commit 목록 확인 : git log --oneline
   그래프까지 확인 : git log --oneline --graph

4) testing을 master로 병합하기 : git merge master

5) testing branch 삭제하기 : git branch -d testing
```

### commit 메세지 수정

- 앞전 메시지일 경우 : git commit --amend

- 전전 메시지일 경우 :
```
git log 
reword, esc shitf + :  / 원하는 메시지 고치기 / wq
git rebase -i HEAD~3 (위에서 세번째) 
```

### 다른 사람 레퍼지토리 가져오기 (다른사람 github에 있는 코드, 내용 그대로 가져오고 싶을때)
- fork -> git bash -> git clone url

