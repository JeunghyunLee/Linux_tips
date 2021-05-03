# Linux_tips
### Tips for using terminal 

#### 1. local terminal에서 서버 접속시 단축키 설정 방법
: alias: ~/.bash_profile에 입력

  1) vim ~/.bash_profile 입력해서 bash profile 있는지 확인
  2) profile 상단에 그대로 작성:: alias ccsl1=‘ssh -p 7777 jhlee4991@@ccsl1.snu.ac.kr’
  3) bash 재실행 혹은 source ~/.bash_profile 실행해서 아무 에러 메시지가 나오지 않으면 성공!

다른 방법
  1) vim ~/.ssh/config 
  2) Host ccsl1, Hostname ccsl1.snu.ac.kr, User jhlee4991, Port 7777 


#### 2. local terminal 글자 색깔 설정 방법
: bash_profile 수정해주기

export CLICOLOR=1
export LSCOLORS=ExFxCxDxBxegedabagacad
export TERM="xterm-color"
#### PS1='\[\e[0;33m\]\u\[\e[0m\]@\[\e[0;32m\]\h\[\e[0m\]:\[\e[0;34m\]\w\[\e[0m\]\$' --> 이 부분은 slack 확인


source .bash_profile하면 적용 완료!

# Github Tips
### Branch
  1) Branch 만들기: `git branch <name>`
  3) master -> branch로 가기: `git checkout <name>`
  4) branch에서 작업하기
  5) branch 에 add, commit, push
  6) 만약 branch 최초의 push라면: `git push --set-upstream origin <name>`
  7) master로 이동: `git checkout master`
  8) merge: `git merge <branch name>`
  9) pull -> push 
  10) branch 삭제: `git branch -d angel`
