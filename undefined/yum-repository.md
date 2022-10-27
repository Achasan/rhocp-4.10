# 🔖 Yum Repository 생성

OpenShift yum repo를 사용하기 위해서는 RHEL Subscription이 되어있는 계정이 필요하다.

*   Subscription 계정 등록

    `rpm --import /etc/pki/rpm-gpg/rpm-gpg-key-redhat-release`

    `subscription-manager register`

<pre><code><strong>[root@bastion ~]# subscription-manager register
</strong><strong>id: xxxxxx
</strong><strong>pw: xxxxxxxxx</strong></code></pre>

*   Yum Repository 등록

    `subscription-manager repos --enable=rhel-8-for-x86_64-baseos-rpms`

    `subscription-manager repos --enable=rhel-8-x86_64-baseos-rpms`

    입력 후 `yum repolist` 입력하여 적용되어있는지 확인
*   적용 후 기본 유틸 설치

    `yum -y install yum-utils net-tools podman wget tar`

