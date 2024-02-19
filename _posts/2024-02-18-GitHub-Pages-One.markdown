---
layout: post #_layouts의 post.html 
title: GitHub Pages 만들기 (1)
date: 2024-02-18 14:00:00 +0900 #_posts의 markdown 날짜와 무조건 일치해야 한다.
description: GitHub을 이용해 정적(Static) 페이지(Page) 만드기 # 내용 요약 (생략 가능)
img: /GitHubPages/github-pages.jpg # assets/img의 img이름
fig-caption: GitHub Pages 로고 입니다. # 이미지에 대한 설명 (생략 가능)
tags: [VSCode, GitHub Pages, Ruby]
---
* 목표
  * 누구나 쉽게 따라할 수 있도록, 최대한 쉽게 설명하기
  * GitHub 사이트를 이용한 정적(Static) 웹사이트를 만들고 + Ruby를 다운받아 보자!
<hr>

##  GitHub Pages란?
GitHub Pages는 GitHub의 리포지토리에서 파일을 직접 가져와 웹 사이트를 게시하는 정적(Static) 사이트 호스팅 서비스이다.

## GitHub Pasges 준비물
* GitHub Repository
* Jekyll
* 템플릿 다운로드 및 적용하기

## GitHub 저장소 만들기
* 저장소 만들기<br>
Repository Name : `<사용자이름>.github.io` 입력 후 Create repository 클릭 <br>
(Repository Name 아래의 빨간색 에러는, 글쓴이는 이미 저장소가 존재한다고 알려주는 것이므로 무시해도 상관없다)
![createRepository](/assets/img/GitHubPages/num1.png)

* git clone 해서 폴더 만들어주기
![clone](/assets/img/GitHubPages/num2.png)

* 정적(Static) 페이지 내용 입력하기
1. VSCode에 Clone한 폴더를 열어주고 index.html 만들어주기
2.  index.html에서 `! + Tab` 을 누르면 html코드가 자동으로 완성
3. body에 내용 입력하기 (Hello World!!)
![clone](/assets/img/GitHubPages/num3.png)
<br><br>
* git push해주기
 ```java
// Terminal
git add .
git commit -m "Title"
git push
```
![clone](/assets/img/GitHubPages/num4.png)
* 생성된 index.html파일 확인하기
![clone](/assets/img/GitHubPages/num5.png)

* 정적(Static)  웹페이지 열어보기
1. Settings의 Pages 로 이동
2. 나의 GitHub Site URL 클릭 <br>
(혹시 GitHub Site URL이 없다면, GitHub에서 자동으로 페이지를 만들어 배포해 줄 때까지 잠시 기다려야 한다)
![clone](/assets/img/GitHubPages/num6.png)
<br><br>
* 페이지 생성 완료<br>
![clone](/assets/img/GitHubPages/num7.png)

우리는 이렇게 GitHub 사이트를 이용한 정적(Static) 웹사이트를 만들어 보았다.<br>
<hr>
## Jekyll 이란?
1. GitHub의 설립자 중 하나가 Ruby를 이용해 만든 정적(Static) 웹 생성기이다.
2. GitHub Pages는 Jekyll을 사용하여 웹사이트를 호스팅 할 수 있다.

## Ruby 설치하기 for Windows
1. Google에서 RubyInstaller 검색
2. Download 클릭

* [Download 바로가기](https://rubyinstaller.org/downloads/)
<br>
![clone](/assets/img/GitHubPages/num8.png)
1. 사진과 같은 페이지로 이동이 됐다면,
2. <b>WITH DEVKIT</b>의 제일 위에 있는 installer 클릭
<br><br>

<hr>

## Ruby Installer Setup
* Page 1
  * Select Setup install Mode 에서
  * Install for me only (recommended) 클릭 <br>
![clone](/assets/img/GitHubPages/ruby1.png)  

* page 2
  * I accept the License 선택 후 Next<br>
![clone](/assets/img/GitHubPages/ruby2.png)  

* page 3
  * Install 클릭 <br>
![clone](/assets/img/GitHubPages/ruby3.png)

* page 4
  * Next 클릭 <br>
![clone](/assets/img/GitHubPages/ruby4.png)

* page 5
  * 업로드 <br>
![clone](/assets/img/GitHubPages/ruby5.png)

* page 6 <br>
  * Ruby 설치완료 <br>
![clone](/assets/img/GitHubPages/ruby6.png)
<br><br>

* 명령 프롬프트(cmd)에서 `ruby --version`입력해서 설치한 version의 확인이 가능하다
![clone](/assets/img/GitHubPages/ruby7.png)

<br>
cmd에서 version을 확인했다면 성공적으로 Ruby를 설치한 것이다.<br>
<hr>

[GitHub Pages 만들기 (2)](https://mad-cost.github.io/GitHub-Pages-Two/)



