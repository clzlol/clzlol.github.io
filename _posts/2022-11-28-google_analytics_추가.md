---
layout: post
title: "Google Analytics 연동하기"
date: 2022-11-28 11:10:00 +0900
categories: jekyll update
comments: true
---

## Google Analytics 등록하기
[google analytics][https://analytics.google.com/analytics/web/#/]에 접속하여 측정 시작을 누른 뒤 다음과 같은 과정을 따라 계정 생성을 진행합니다.
![2](\images\2.png)

![2-1](\images\2-1.png)

![2-2](\images\2-2.png)


## 나의 BLOG와 Google Analytics 연동하기
등록을 완료한 다음 관리로 이동하고 데이터 스트림으로 이동한 뒤 플랫폼 선택 창에서 웹을 선택합니다.
![3](\images\3.png)


웹사이트 URL에 Git Blog의 주소(clzlol.github.io)를 입력하고 스트림의 이름을 입력한 뒤 스트림을 만듭니다.
![4](\images\4.png)


그리고 측정 ID를 복사한 뒤 위의 '태그 안내 보기'로 이동합니다.
![5](\images\5.png)


태그 안내 보기 창에서 코드를 복사한 뒤 _layouts 폴더 내의 default.html의 <body> 위에 다음과 같이 붙여넣어줍니다.
![8](\images\8.png)


그리고 Git에 commit, push 후 반영이 되고 사이트에 접속한 뒤 Google Analytics에 접속하면 다음과 같이 정상적으로 접속 수 트래킹이 가능해짐을 알 수 있었습니다.
![9](\images\9.png)