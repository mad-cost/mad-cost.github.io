---
layout: post #_layouts의 post.html 
title: GitHub Pages 만들기 (1)
date: 2024-02-18 14:00:00 +0900 #_posts의 markdown 날짜와 무조건 일치해야 한다.
description: GitHub을 이용해 정적(Static) 페이지(Page) 만드기 # 내용 요약 (생략 가능)
img: /GitHubPages/github-pages.jpg # assets/img의 img이름
fig-caption: GitHub Pages 로고 입니다. # 이미지에 대한 설명 (생략 가능)
tags: [GitHub, Backend, java]
---
## GitHub Pages란?
GitHub Pages는 GitHub의 리포지토리에서 파일을 직접 가져와 웹 사이트를 게시하는 정적(Static) 사이트 호스팅 서비스이다.

## GitHub Pasges 준비물
* GitHub Repository
* Jekyll
* 템플릿 다운로드 및 적용하기

## GitHub 저장소 만들기
![createRepository](/assets/img/GitHubPages/num1.png)
<br>
Repository Name : `<사용자이름>.github.io` 입력 후 Create repository 클릭 <br>
Repository Name 아래의 빨간 에러는, 나는 이미 저장소가 존재한다고 알려주는 것이므로 무시해도 상관없다
<br><br>

![clone](/assets/img/GitHubPages/num2.png)
<br>
git clone 해서 폴더 만들어주기
<br><br>


![clone](/assets/img/GitHubPages/num3.png)
<br>
1. VSCode에 Clone한 폴더 열어주고 index.html 만들어주기
2.  index.html에서 `! + Tab` 을 누르면 html코드가 자동으로 완성된다
3. body에 내용입력 : Hello World!!
<br><br>

![clone](/assets/img/GitHubPages/num4.png)
<br>
터미널을 열고, git push 해주기
```java
<!-- 이제부터 여기는 Terminal 입니다 -->
git add .
git message -m "Title"
git push
```
<br><br>

![clone](/assets/img/GitHubPages/num5.png)
<br>
git push를 제대로 해줬다면 index.html 파일이 생성된 것을 볼 수 있다
<br><br>

![clone](/assets/img/GitHubPages/num6.png)
<br>
1. Settings의 Pages 로 이동
2. 나의 GitHub Site URL 클릭
3. 혹시 GitHub Site URL이 없다면, GitHub에서 자동으로 페이지를 만들어 배포해 줄 때까지 잠시 기다려야 한다.
<br><br>

![clone](/assets/img/GitHubPages/num7.png)
<br>
index.html에 입력한 Hello World!! 확인 완료
<br><br>

이렇게 GitHub 사이트를 이용한 정적(Static) 웹사이트를 만들어 보았다.<br>
[GitHub Pages 만들기 (2)](https://mad-cost.github.io/GitHub-Pages-Two/)



