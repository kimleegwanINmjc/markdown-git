# Git , Markdown
#  Git
## 1.설정과 초기화
> 사용자명/이메일구성
  * git config- -global user.name"Your name"
  * git config- -global user.email"Your email"
> 저장소별 사용자명/이메일 구성하기(디렉터리 이동후)
  * git config user.name “Your name”
  * git config user.email “Your email address”
>전역 설정 정보 조회
  * git config - -global - -list
>새로운 저장소 초기화하기
  * mkdir /path/newDir
  * cd /path/newDir
  * git init
>저장소 복제
  * git clone <저장소 url>
>새로운 원격 저장소 추가하기
  * git remote add <원격 저장소> <저장소 url>
* * *
## 2.기본적인 사용법
> 새로운 파일을 추가하거나 존재하는 파일 스테이징하고 커밋하기
 * git add <파일>
 * git commit -m “<메시지>”
>add 명령에서 Git 대화 모드를 사용하여 파일 추가하기
 * git add -
> 파일의 변경 사항 스테이징하기
 * git add -u 
> 모든 파일의 변경 사항 커밋하기
 * git commit -m “<메시지>” -a
 * * *
 ## 3.브랜치
> 브랜치 목록 보기
 * git branch
 * git branch -r
 * git branch -a
> 체크아웃하기
 * git checkout <브랜치>
 * git checkout -b <브랜치>
 * git checkout -f<브랜치>
 * git checkout -m -M<브랜치>
>다른 브랜치를 현재 브랜치로 합치기
 * git merge <브랜치>
>커밋하지 않고 합치기
 * git merge - -no-commit <브랜치>
>선택하여 합치기
 * git cherry-pick <커밋명>
>브랜치 삭제하기
 * git branch -d <삭제할 브랜치>
 * git branch -D <삭제할 브랜치>
 
