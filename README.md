# Lab6 Lecture Note
---
##Git   
- 직관적이고 편리한 **Version Control & Collaboration** 소프트웨어.         
- Main Branch에 작업한 Branch를 Merge 시키는 방식 (2주차 Github 강의 참고)

ex) 소프트웨어 개발 혹은 문서 작업 시 하는 Basic solution -    
프로젝트_최종.txt   
프로젝트_최종_수정1.txt   
프로젝트_최종_수정1_진짜최종.txt   
프로젝트_최종-수정1_진짜최종_추가수정2.txt   
...   
공간 낭비 뿐만 아닌 알아 보기 힘든 방식이다.   
Collaboration 방면에서도 비효율적이므로 Git을 사용함.   

---

Changes Vs. Snapshots
Changes - 기본 버전에 대한 변경 사항으로 데이터를 저장하는 방식   
Snapshot - 특정 시점의 데이터 이미지를 생성하여 저장하는 방식   

1. Local : 버전 로컬(개인) 컴퓨터에 저장. 협업 불가.   
2. Centralized : 중앙 서버에서 버전 관리. 의존성 문제가 있음.   
3. Distributed : 중앙 서버 뿐만 아니라 로컬 컴퓨터도 데이터베이스를 소유. Centralized 방식의 단점을 보완
   
Git의 세가지 상태 **중요!   
1. Modified : Working Directory의 내용을 중간 단계인 Staging Area로 옮김.
2. Staged : Staging Area. Commit 단계로 가기 위한 점검.
3. Commmitted : .git directory (Repository)에 특정 시점 기록됨.

$ git init : 현재 디렉토리에 새로운 repository 생성   
$ git status : 어떤 상태인지 알 수 있다.   
$ git add [file_name] : 파일 생성. ex) git add README.md   
- git add . : working directory 에 있는 모든 파일을 Staging Area로 이동시킴.
- git rm --cached [file_name] : 커밋시키지 않고 싶은 파일을 빼는 명령어(Unstaging)
- nano .gitignore : 무시할 파일을 입력

$ git commit -m "committing message" : 커밋 단계 명령어.  커밋 메세지를 입력   
$ git log : 커밋한 로그 리스트를 보여줌.   

