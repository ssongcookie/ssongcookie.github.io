---
layout: post
title:  "Github 블로그 만들기!"
date:   2023-08-31 13:10:00 +0900
categories: [Github, blog]
typora-root-url: ../
---
### 목차
1. git repository 생성
2. clone 하기
3. ruby 설치
4. jekyll 설치
5. bundle install
6. Jekyll을 로컬서버에 띄우기
7. 원격에 push

---
## [1. git repository 생성]  

| ![git_repository](/assets/img/git_repository_01.png) | 
|:--| 
|  Repository 이름 설정 시 저장소의 [username]부분이 사용자 이름과 정확히 일치하지 않으면 작동하지 않을 수 있다. |

<br><br>

---  
## [2. clone 하기]  
- git bash를 열어 clone할 경로로 이동한 후, clone을 시작한다. 그리고 Push 한다.  
<br>
- 명령어  
```md
cd /[username].github.io/  
echo "Hello World" > index.html  
git add --all  
git commit -m "Initial commit"  
git push -u origin main  
```
 
| ![git_clone_push](/assets/img/git_clone_push_01.png) |
|:--:|
| 잘 Push되었으면 주소창에 username.github.io를 입력하여 확인한다. |

<br><br>

---
## [3. ruby 설치]
- ruby 홈페이지 : [rubyinstaller](https://rubyinstaller.org/downloads/){:target="_blank"}

| ![git_build_error](/assets/img/git_build_error.png) |
|:--:|
| 최신 버전은 호환이 되지 않을 수 있으니 안전하게 2.7 정도의 버전을 설치한다. |

| ![git_build_success](/assets/img/git_build_success.png) |
|:--:|
| 실제로 최신 버전으로 진행 시 build 에러가 발생했고, 버전을 2.7.8 로 설치 후 다시 push 하니 정상적으로 build 되었다. |

<br><br>

---
## [4. jekyll 설치]
```md
gem install jekyll
```
- Start Command Prompt with Ruby를 실행하고, 위 명령어를 실행한다.
- ruby -v 와 jekyll -v로 정상적으로 설치되었음을 확인한다.

<br><br>

---
## [5. bundle install]
```md
bundle install
```
- 위 명령어를 실행한다.

<br><br>

---
## [6. Jekyll을 로컬서버에 띄우기]
```md
bundle exec jekyll serve
```  
  
| ![bundle_server](/assets/img/bundle_server.png) |
|:--:|
| 위 명령어를 실행하고, 로컬서버를 확인한다. |

<br><br>

---
## [7. 원격에 push]
```md
git add --all
git commit -m "커밋 메시지"
git push
```
- 위 명령어로 원격에 push 하고, 브라우저에 github.io 주소를 입력하여 확인한다.



