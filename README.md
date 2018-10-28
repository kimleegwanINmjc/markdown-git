# Git , Markdown
#  Git
## 1.설정과 초기화
> 사용자명/이메일구성
1. git config- -global user.name"Your name"
2. git config- -global user.email"Your email"
> 저장소별 사용자명/이메일 구성하기(디렉터리 이동후)
1. git config user.name “Your name”
2. git config user.email “Your email address”
>전역 설정 정보 조회
git config - -global - -list
>새로운 저장소 초기화하기
mkdir /path/newDir
cd /path/newDir
git init
>저장소 복제
git clone <저장소 url>
>새로운 원격 저장소 추가하기
git remote add <원격 저장소> <저장소 url>
