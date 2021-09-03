---
title : "다양한 인터넷 기초 지식 (Other Internet Knowledge)"
categories:
  - Basic Web knowledge
tags:
  - internet
toc: true
toc_sticky: true
toc_label: "Contents"
---

# 다음날이 도래했다.

9월의 시작입니다. 2학기 개강도 시작했습니다.

개발 공부하기도 빡센데 대학 강의에, 인턴 준비에.... 시간이 너무 없다는 것을 느끼는 요즘입니다. 진작에 공부하고 뭐라도 좀 할 껄, 이라는 생각이 머리 속을 떠나지를 않네요.

하지만 아직 늦지 않았습니다. 그리고 늦었음 어떻습니까. 그냥 하면 되는 거지. 늦었다고 죽을 수는 없잖아요?

오늘도 열심히 포스팅 해보겠습니다. 남은 5가지 Internet Web 기초를 한꺼번에 끝내겠습니다. 

**자, 드가자~**



<br/><br/>
# What Is HTTP?

## HTTP protocol

먼저 `프로토콜`이라는 용어부터 살펴보자.

`프로토콜`이란, 복수의 컴퓨터 사이나 중앙 컴퓨터와 단말기 사이에서 데이터 통신을 원활하게 하기 위해 필요한 통신 규약이다. 즉, 다른 컴퓨터와 소통하기 위해 정해놓은 하나의 양식인 것이다. 회사에서 보고서를 주고받을 때 정해진 양식이 있듯이 말이다.

그렇다면 `HTTP`는 무엇일까.

`HyperText Transfer Protocol`의 약자로, web 기반의 앱들이 서로 통신하고 데이터를 교환하게 만들어주는 `application layer protocol`이다. 즉, 웹의 메신저 역할을 하며 콘텐츠, 이미지, 비디오 등을 옮기는 기능을 수행한다.

참고로 HTTP는 TCP/IP 기반의 프로토콜이다. TCP/IP이 무엇이고 왜 배우는지 몰랐는데, 이제야 알 것 같다. HTTP를 자세히 알기 위함이었다.

## Three Important things about the HTTP

HTTP의 3가지 특징에 대해서 알아보자.

**1. HTTP는 connectionless하다.**  
request를 한 뒤, client는 server와 연결이 끊어지며, responce를 받을 때 연결connection이 재구축된다.

**2. 통신하는 컴퓨터들끼리 HTTP를 읽을 수 있는 한, HTTP는 그 어떤 정보도 전송할 수 있다.**

**3. HTTP는 stateless하다.**  
client와 server는 현재 http로 통신할 때에만 서로를 알고 있다. 만약 통신이 닫히고 두 컴퓨터가 다시 연결을 하고 싶다면, 서로에게 다시 한번 정보를 제공해야 하며 이 연결은 마치 처음 것과 같이 처리된다.

## Why The HTTP?

HTTP는 처음에는 HTML만을 주고받은 목적으로 만들어졌으나, 계속 진화하고 기능들이 추가되며 현재는 가장 빠르고 신뢰할 수 있는, 웹에서 데이터를 옮기는 가장 좋은 방식이 되었다.

## HTTP Structure

HTTP는 데이터를 전송하거나 request할 떄, 관련된 데이터를 함께 넣는다. 그래서 Headers와 Body로 구분되며, Headers에서 request 대상과 전송 방식에 대해 기술한다.



<br/><br/>
# How Do Web Browers Work?

브라우저 작동 방식은 지금 수준에 굳이 필요 없으므로 짧게 넘어가겠습니다.

브라우저는 User Interface, Brouser Engine, Rendering engine, JS interpreter 등등 다양한 시스템으로 구조화되어 있습니다.

여기서 브라우저가 구동하는 순서는 이렇습니다.

**1. Resource Gathering**  
브라우저가 웹페이지를 구성하기 위해 서버에서 html, css, js 같은 리소스들을 가지고 옵니다.

**2. Parse HTML & Create DOM Tree**  
html을 DOM 트리 구조로 변환시킵니다.

**3. Create Render Tree From DOM Tree**  
이제 html 파일을 css와 결합시킨 Render 트리를 만듭니다.

**4. Layout**  
Render 트리를 각 box 또는 inline 요소로 변환시키고 브라우저에서 차지할 위치, 크기를 계산합니다.

**5. Painting**  
이제 마지막으로 브라우저에 최종 내용을 그래픽 처리합니다.


<br/><br/>
# 배울 게 너무 많다...

솔직히 그 밖에도 'How DNS Works Visualy'나 'What is Web Hosting?' 같은 것도 들었는데 글로 쓰기가 힘이 부치네요....

블로그 포스팅하시는 모든 분들에게 존경의 말씀을 전합니다....