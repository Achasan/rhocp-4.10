# π₯ ESXi λΈλ μμ±

## ESXi VM μ€μ 

* μ¬λ΄ ESXi κ³μ 
  * ID: ----
  * PW: ------------
*   λ‘κ·ΈμΈ ν μ μ νλ©΄

    <figure><img src="../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>


*   \[VM μμ±/λ±λ‘] ν΄

    <figure><img src="../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>


*   μ΄λ¦ λ° κ²μ€νΈ μ΄μ μ²΄μ  μ ν

    <figure><img src="../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>


*   μ€ν λ¦¬μ§ μ ν

    <figure><img src="../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>


*   VM μ€ν μ€μ 

    * CPU: 4 Core
    * RAM: 16GB
    * Disk: 120GB
    * Network Adapter: Internal Network
    * νλλμ€ν¬: **μ¬ νλ‘λΉμ λ λ¨ μ²΄ν¬ (λμ ν λΉ)**
    * CD/DVD λλΌμ΄λΈ 1: μ€ν λ¦¬μ§μ μλ‘λ λμ΄μλ ISOλ‘ λΆνν  μ μλλ‘ μ€μ  (Datastore1)

    <figure><img src="../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>


* VM μ€ν ν RHEL 8.5 λ²μ  μ€μΉ, λ€νΈμν¬ μ€μ 
  * Manual
  * 172.16.0.241/24
  * G/W: 172.16.0.1
  * DNS: 172.16.0.241 / 8.8.8.8\
    (OpenShift μ€μΉ νμΌ λ€μ΄ λ°μ λλ 8.8.8.8 μ¬μ©, λ€νΈμν¬ κ΅¬μ± ν μ€μΉ μμλ 172.16.0.241λ‘ μ€μ )
