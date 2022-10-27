---
description: 로컬 레지스트리 미러링(httpd) 및 openshift 설치 파일 다운로드
---

# 레지스트리 미러링(httpd),설치파일 다운로드

## Httpd 구성

*   repo 구성을 위한 Apache 설치

    `yum -y install httpd`

    `cd /var/www/html`

    `ln -s /yumrepo /var/www/html`\
    &#x20;`` ⇒ `/var/www/html/yumrepo` 디렉토리와 `/var/www/html` 를 링크시킴

    `vi /etc/httpd/conf/httpd.conf` \
    &#x20;  ⇒ `Listen 8080` 포트 8080 변경
*   httpd 활성화

    `systemctl enable --now httpd`

    `systemctl status httpd`
*   OpenSSL 생성하기

    ``
