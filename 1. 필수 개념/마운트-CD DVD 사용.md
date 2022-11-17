# 마운트-CD DVD 사용.md
물리적인 장치를 특정한 위치와 연결하는 과정.  
(일반적으로 디렉터리와 연결한다)

## X윈도우에서 마운트

## 텍스트 환경에서 마운트
VMWare를 사용하는 경우 맨 처음에 설치할때 했던 것처럼 장치 설정에서 ISO파일을 투입한다.  
Player가 실행중이라면, 좌상단 Player > Removable Devices > CD/DVD(SATA) > Settings 로 메뉴에 진입  

CD를 넣으면 자동으로 D:든 E:든 연결이 되지만,  
X윈도우 환경이면 이상한 데로 연결되는 경우가 많고,  
텍스트 환경이면 자동 연결이 안 된다.  
꼭 수동으로 연결을 해야 한다.



### 순서

```
umount /dev/cdrom
```
(자동 연결된) 마운트를 해제
[*]dev : device

```
mkdir /media/cdrom
```
디렉토리 생성

```
mount /dev/cdrom /media/cdrom/
```
수동 마운트

```
cd /media/cdrom/
```
CD/DVD 내부로 이동

&nbsp;  

(작업 후)

&nbsp;  

```
cd
```
루트로 이동

```
umount /dev/cdrom
```
마운트 해제

&nbsp;  

가상 머신을 사용하는 경우 setting에서 CD/DVD 해제까지.  
(Setting 안 들어가고 Disconnect 하면?)
