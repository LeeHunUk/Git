# Git + GitHub

## 1. Git이란?
> Git(깃)은 컴퓨터 파일의 변경사항을 추적하고 여러 사용자들 간에 해당 파일 작업을 조율하기 위한 대표적인 버전 관리 시스템

## 2. 시작하기 전 확인사항
> 터미널을 열고 git 버전을 확인하여 설치 되어있지 않다면 설치 후 진행하시기 바랍니다.   
> https://git-scm.com/
> 설치 후 GitHub 가입 후 진행하시면 됩니다.
```sh
 User $ git --version
```

## 3. 사용자 정보 등록
```sh
 # Git 사용자 정보 확인
 User $ git config --global --list
 
 # Git 사용자 정보 등록
 User $ git config --global user.name '사용자 이름'
 User $ git config --global user.email '깃허브 이메일 주소'
 User $ git config --global core.autocrlf true(mac일 경우 input)
```

## 4. 버전 생성
```sh
 # 현재 프로젝트를 버전 관리 시작선언
 User $ git init
 
 # Git 현재 상태 확인
 User $ git status
 
 # Git을 통해 버전의 추적을 추가
 User $ git add . (모든 파일 폴더 추적)
 User $ git add 파일명 (해당 파일 또는 폴더 추적)
 
 # Git 버전 생성(-m : 메세지를 추가한다는 의미)
 User $ git commit -m '히스토리 만들기'
 
 # Git 기록 확인
 User $ git log
```

## 5. 코드 업로드
```sh
 # Github repository랑 내 로컬 프로젝트랑 연결
 User $ git remote add origin github주소(ex : https://github.com/LeeHunUk/Git.git)
 
 # 연결이 잘 되었는지 확인
 User $ git remote -v
 
 # GitHub 업로드
 User $ git push origin master
```

## 6. 브랜치
```sh
 # branch 생성
 User $ git branch 브랜치명
 
 # branch 확인
 User $ git branch
 
 # branch 변경
 User $ git checkout 브랜치명
 
 # branch 삭제(현재 브랜치는 삭제 x)
 User $ git branch -d 브랜치명
 
 # branch 생성하자 마자 이동
 User $ git checkout -b 브랜치명
 
 # branch 끼리 병합
 User $ git merge 병합하고자하는브랜치명

 # 버전 되돌리기
 User $ git reset --hard HEAD~ 되돌릴단계 ex)git reset --hard HEAD~3
 User $ git reset --hard 커밋아이디값
 
 # 브랜치 업로드(origin 별칭은 변경이 가능하나 통상적으로 origin을 사용)
 User $ git remote add origin github주소(ex : https://github.com/LeeHunUk/Git.git)
 
 User $ git push origin 브랜치명 
 or
 User $ git push origin --all
```

## 7. Clone
```sh
 User $ git clone github주소 폴더명
```



















