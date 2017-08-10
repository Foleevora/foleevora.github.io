---
layout: post
title: HTTP vs HTTPS
---

HTTP는 HyperText Transfer Protocol의 줄임말이고 HTTPS는 HyperText Transfer Protocol over Secure sockets layer의 줄임말입니다.

HTTPS는 HTTP에서 secure sockets layer가 붙은 프로토콜이라고 합니다.

secure sockets layer(SSL)이라고 불리는 것은 보안 소켓 계층이라고 하는데 이 SSL 유무가 HTTP와 HTTPS의 차이점이라고 할 수 있죠. 

이전 포스팅에도 알 수 있듯 
<https://foleevora.github.io/HTTP/>

HTTP는 우리가 인터넷을 사용하면서 적게되는 개인 정보들을 서버에 보내는데 아무 보안 장치 없이 보냅니다. 

(예를 들면 foleevora1234라고 입력하고 전송하면 foleevora1234 그대로 서버에 전송)

따라서 보안상 문제가 있었습니다. 그래서 SSL을 붙인 프로토콜인 HTTPS를 만든거죠.

HTTPS는 서버에 전송하는 모든 정보를 전부 암호화해서 전송합니다. 

****

HTTPS를 사용하는 홈페이지는 SSL 인증서를 필수적으로 발급받으면 사용자는 브라우저를 통해 인증서에 대한 정보를 확인할 수 있습니다. 

발급 받는 인증기관은 여러곳이 있지만 글로벌사인, VeriSign, 지오트러스트 등이 있다네요.

이 인증서를 통해 사용자는 해당 사이트가 신뢰할 수 있는 사이트임을 확인할 수 있습니다. 

SSL의 암호화 기법으로는 공개 키 방식을 사용하는데 여기서 공개 키 방식이란

    공개 키 방식은 공개, 비공개 키를 각각 하나씩 만들고
    사용자들의 데이터는 공개키로 암호화를 하여 서버로 전송하고
    복호화는 비공개 키를 아는 서버만이 가능하기 때문에
    서버 전송 도중에 데이터가 유출되어도 복호화 불가능.

HTTPS를 사용하면 사이트가 느려지기 때문에 데이터를 전송하지 않는 페이지에서는 HTTP를 쓰다가 로그인 등 데이터를 전송하는 페이지에서는 HTTPS를 사용한다고 합니다.


