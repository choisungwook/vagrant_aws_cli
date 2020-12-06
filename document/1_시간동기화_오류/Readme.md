# 오류
* aws와 시간 동기화가 안되어 인증 오류 발생

![](./error.jpg)

<br>

# 해결
* ntpdate명령어로 시간 동기화

```sh
sudo yum install ntp
sudo yum install ntpdate
sudo ntpdate pool.ntp.org
```