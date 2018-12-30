---
categories: Linux
---

## apache Service Port 변경
apache 2 버젼 기준으로.

    1. 아파치의 포트 관련 환경설정 파일 수정
    $sudo vi /etc/apache2/ports.conf
    안에 Listen 80 을 원하는 포트 no로 수정
    ex: Listen 8080
    
    2. 아파치의 가상호스트 환경설정 파일 수정
    $sudo vi /etc/apache2/sites-available/000-default.conf
    안에 <VirtualHost *:80> 을 원하는 포트 no로 수정
    ex: <VirtualHost *:8080>
    
