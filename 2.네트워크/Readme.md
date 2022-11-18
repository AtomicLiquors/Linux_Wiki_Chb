
우분투는 랜카드를 ens32 또는 ens33으로 할당한다.
```
ifconfig ens32 
ifdown ens32
ifup ens32
```
- ifconfig *Interface Configuration* : 장치의 IP주소 설정 정보 출력
- down : 정지
- up : 가동

&nbsp;  

### nm-connection-editor / nmtui
네트워크 관련 대다수 작업을 수행하는 명령어.

&nbsp;  

### systemctl
네트워크 설정 변경 후 변경 내용을 적용시키는 명령어.
```
systemctl start
systemctl stop
systemctl restart
systemctl status
```

###nslookup
DNS서버 작동을 테스트

&nbsp;  


## 주요 설정 파일
- X윈도 : /etc/NetworkManager/system-connections/ 
- CLI : /etc/netplan/*.yaml 파일

### /etc/resolv.conf
DNS 서버의 정보 및 호스트 이름이 들어있는 파일  
단 DNS 서버 정보를 영구적으로 변경하려면 nm connection editor 커맨드나 netplan/yaml 파일 변경을 해야 한다.

### /etc/hosts
현 컴퓨터의 호스트 이름 및 FQDN이 들어있는 파일
