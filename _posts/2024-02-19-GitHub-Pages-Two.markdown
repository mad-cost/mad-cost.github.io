---
layout: post #_layouts의 post.html 
title: GitHub Pages 만들기 (2)
date: 2024-02-19 08:00:00 +0900 #_posts의 markdown 날짜와 무조건 일치해야 한다.
description: GitHub을 이용해 정적(Static) 페이지(Page) 만드기 # 내용 요약 (생략 가능)
img: /GitHubPages/github-pages.jpg # assets/img의 img이름
fig-caption: GitHub Pages 로고 입니다. # 이미지에 대한 설명 (생략 가능)
tags: [Jekyll, Ruby, GitHub]
---
* 목표
  *  누구나 쉽게 따라할 수 있도록, 최대한 쉽게 설명하기
  * Jekyll을 설치하고 + 템플릿을 적용해보자!
<hr>


## Jekyll 설치하기
* Gem을 이용하여 Jekyll 설치해보자
1. VSCode로 돌아와 터미널 열어주기
2. 터미널에 Jekyll을 작동시키기 위한 명령어 3가지 입력
```java
// Terminal
gem install bundler
gem install github-pages
gem install jekyll
```
(의존성 다운로드에 시간이 걸릴 수 있으니 조금만 기다려주자)
![clone](/assets/img/GitHubPages/num9.png)

* Jekyll의 프로젝트 구조와 파일 생성하기
1. index.html파일 삭제하기 <br>
![clone](/assets/img/GitHubPages/num10.png)
2. 터미널에 `jekyll new .`입력 <br>
( `jekyll new .`라는 명령어 자체가 내부에 파일이 존재하면 실행이 되지 않는 명령어이다)
```java
// Terminal
jekyll new .
```
3. 폴더에 새로운 파일들이 생기는 것을 볼 수 있다<br>
![clone](/assets/img/GitHubPages/num11.png)
<br><br>

* 사이트 모습 확인하기
1. 터미널에 순서대로 `bundle install`, `bundle exec jekyll serve`를 입력해주기
```java
// Terminal
bundle install
bundle exec jekyll serve
```
2.  터미널에 Server address `Ctrl + Click` 해주기
![clone](/assets/img/GitHubPages/num12.png)
3. 사이트 연결 완료
![clone](/assets/img/GitHubPages/num13.png)

이로써 우리는 Jekyll을 이용해서 사이트를 만들어 보았다.
<hr>

## 템플릿 테마 적용하기

Jekyll은 여러가지 테마를 입힐 수 있다.<br>
1. [Jekyll Themes 바로가기](https://jekyllrb.com/docs/themes/)
2. [My Themes 바로가기](https://jekyllthemes.io/theme/flexible-jekyll)

* 테마 받아오기
1. 체크한 부분 클릭해서 GitHub으로 이동 
![clone](/assets/img/GitHubPages/num14.png)
2. ZIP 다운받고, 압축 풀어주기
![clone](/assets/img/GitHubPages/num15.png)
3. VSCode 폴더의 기존에 있던 파일들을 모두 삭제하고,
4. ZIP 압축 해제한 모든 파일 폴더에 넣어주기
![clone](/assets/img/GitHubPages/num16.png)
5. 내 정보로 수정하기<br>
기존에 있던( `_config.yml` )의 정보를 내 정보로 수정해보자<br>
Img는 `assets/img`에서 확인이 가능하다 
6. 사이트 모습 확인<br>
수정한 테마의 사이트 정보를 확인해보자
```java
// Terminal
bundle install
bundle exec jekyll serve
```
![clone](/assets/img/GitHubPages/num17.png)
7. GitHub에 저장하고, 적용된 테마 확인하기
```java
// Terminal
git add.
git commit -m "완료"
git push
```
![clone](/assets/img/GitHubPages/num19.png)
<br><br>
![clone](/assets/img/GitHubPages/num18.png)

이렇게 GitHub Pages 만들기를 완성해 보았다.<br>
처음 하는 사람도 따라 할 수 있도록 최대한 쉽게 설명하였는데, 다들 성공했을 거라고 믿어 의심치 않는다😊