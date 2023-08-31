---
layout: post
title:  "Github 블로그 만들기!"
date:   2023-08-31 13:10:00 +0900
categories: [Github, blog]
typora-root-url: ../
---
Github 블로그 만들기! 
<br><br><br>

- [git repository 생성]
<br> 
| ![git_repository](/assets/img/git_repository_01.png) | 
|:--:| 
|  Repository 이름 설정 시 저장소의 [username]부분이 사용자 이름과 정확히 일치하지 않으면 작동하지 않을 수 있다. |
<br><br><br>
  
- [clone 하기]  
- git bash를 열어 clone할 경로로 이동한 후, clone을 시작한다. 그리고 Push 한다.  
<br><br><br>
 
- [명령어]  
- cd /[username].github.io/  
- echo "Hello World" > index.html  
- git add --all  
- git commit -m "Initial commit"  
- git push -u origin main  
<br>

| ![git_clone_push](/assets/img/git_clone_push_01.png) |
|:--:|
| 잘 Push되었으면 주소창에 username.github.io를 입력하여 확인한다. |
<br><br><br>

- [ruby 설치]
- ruby 홈페이지 : [rubyinstaller](https://rubyinstaller.org/downloads/){:target="_blank"}
<br>
| ![git_build_error](/assets/img/git_build_error.png) |
|:--:|
| 최신 버전은 호환이 되지 않을 수 있으니 안전하게 2.7 정도의 버전을 설치한다.<br>
=> 실제로 웹호스팅 build 에러가 발생했고, 버전은 2.7.8 로 설치 후 다시 push 하니 정상적으로 build 되었다. |
<br>
| ![git_build_success](/assets/img/git_build_success.png) |
<br><br><br>

- [jekyll 설치]
- gem install jekyll
- Start Command Prompt with Ruby를 실행하고, 위 명령어를 실행한다.
- ruby -v 와 jekyll -v로 정상적으로 설치되었음을 확인한다.
<br><br><br>

- [bundle install]
- bundle install
- 위 명령어를 실행한다.
<br><br><br>

- Jekyll을 로컬서버에 띄우기
- bundle exec jekyll serve
<br>
| ![bundle_server](/assets/img/bundle_server.png) |
|:--:|
| 위 명령어를 실행하고, 로컬서버를 확인한다. |
<br><br><br>

- [원격에 push]
- git add --all
- git commit -m "커밋 메시지"
- git push
<br>
- 위 명령어로 원격에 push 하고, 브라우저에 github.io 주소를 입력하여 확인한다.



