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
* * *
## 4.이력
>모든 이력 보기
 * git log
>현재 작업 트리와 인덱스의 차이점 보기
 * git diff
>파일의 커밋 정보 줄 단위로 보기
 * git blame <파일>
* * *
## 5.원격저장소
>저장소 복제하기
 * git clone <저장소>
>새로운 원격 저장소 추가하기
 * git remote add <원격 저장소> <저장소 url>
>원격 저장소에서 합치지 않고 지역 브랜치로 변경 사항 
 * git fetch <원격 저장소>
>원격 저장소에서 변경 사항을 가져와 현재 브랜치에 합치기
 * git pull <원격 저장소>
>새로운 로컬 브랜치를 원격 저장소에 푸싱하기
 * git push <원격 저장소> <지역 브랜치>
>원격 저장소에서 쓸모가 없어진 원격 브랜치 제거하기
 * git remote prune <원격 저장소>
>원격 저장소를 제거하고 관련된 브랜치도 제거하기
 * git remote rm <원격 저장소>
* * *
# Markdown
## 1.제목(Heading)
문서를 작성할 때 가장 기본이 되는 제목은 HTML의 h1~h6 태그와 유사합니다.
<pre><code># Heading</code></pre>
 # Heading 
<pre><code>### Heading</code></pre>
 ### Heading
## 2. 본문
HTML의 p 와 같은 본문은 텍스트를 그대로 작성하면 됩니다.
## 3.인용
인용은 '>'를 넣어서 작성합니다
<pre><code>>안뇽하세여</code></pre>
>안뇽하세요
>>안뇽하세요
## 4.리스트
 ### 4.1순서가 없는 리스트
  '*' 또는 '-'를 사용해서 순서가 없는 리스트를 작성할 수 있습니다. 'tab' 또는 2칸 띄어쓰기를 통해 중첩된 항목을 작성할 수 있습니다.
  <pre><code>
  *항목1
  *목항
  *사랑
   *안프</code></pre>
 * 항목1     
 * 목항      
 * 사랑     
  * 안프   
 - 항목1     
 - 목항      
 - 사랑     
  - 안프   
