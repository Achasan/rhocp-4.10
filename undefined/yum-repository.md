# ๐ Yum Repository ์์ฑ

OpenShift yum repo๋ฅผ ์ฌ์ฉํ๊ธฐ ์ํด์๋ RHEL Subscription์ด ๋์ด์๋ ๊ณ์ ์ด ํ์ํ๋ค.

*   Subscription ๊ณ์  ๋ฑ๋ก

    `rpm --import /etc/pki/rpm-gpg/rpm-gpg-key-redhat-release`

    `subscription-manager register`

<pre><code><strong>[root@bastion ~]# subscription-manager register
</strong><strong>id: xxxxxx
</strong><strong>pw: xxxxxxxxx</strong></code></pre>

*   Yum Repository ๋ฑ๋ก

    `subscription-manager repos --enable=rhel-8-for-x86_64-baseos-rpms`

    `subscription-manager repos --enable=rhel-8-x86_64-baseos-rpms`

    ์๋ ฅ ํ `yum repolist` ์๋ ฅํ์ฌ ์ ์ฉ๋์ด์๋์ง ํ์ธ
*   ์ ์ฉ ํ ๊ธฐ๋ณธ ์ ํธ ์ค์น

    `yum -y install yum-utils net-tools podman wget tar`

