---
layout:            post
title:             "Node Express"
menutitle:         "Node Express"
date:              2020-04-21 14:00:00 +0900
tags:              Node.js Node
category:          Node
author:            charllossDev
cover:             /assets/mountain-alternative-cover.jpg
published:         true
redirect_from:     "/Node-Basic-Redirect/"
cover:             /assets/mountain-alternative-cover.jpg
language:          EN
comments:          true
math:			         false
---

# 서드파티 라이브러리 모듈


## Application
* 익스프레스 인스턴스를 어플리케이션이라고 한다.
* 서버에 필요한 기능인 미들웨어 어플리케이션에 추가한다.
* 라우팅 설정을 할 수 있다.
* 서버를 요청 대기 상태로 만들 수 있다.

##  Middleware
* 미들웨어는 함수들의 연속
* 로깅 미들웨어
  + 서드파티 미들웨어
  + [morgan](https://www.npmjs.com/package/morgan)
* 에러 미들웨어
  + 파라메터를 통해 일반 미들웨어와 에러 미들웨어를 구분한다.

## Router
* express에서는 어플리케이션이(get(), post() 메서드를 통해) router를 사용하여 라우팅을 처리하여 Api를 관리한다.
* API가 많이지면, 별로도 관리를 할 수 있는 라우터 클래스틑 통해 관리를 할 수 있다.
