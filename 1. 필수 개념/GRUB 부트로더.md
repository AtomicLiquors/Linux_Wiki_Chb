# GRUB 부트로더
GNU 프로젝트의 부트로더이다. 웬만한 운영 체제의 커널을 불러올 수 있으며, 인자를 넘겨 줄 수도 있다.
- 부트정보를 사용자가 임의로 변경 가능하다. (부트정보가 올바르지 않아도 수정할 수 있다.)
- 다른 운영체제와 멀티부팅이 가능하다. (잘 쓰지 않음)
- 대화형 설정 : 커널 경로와 파일 이름만 알면 부팅 가능

## GRUB2
- 셸 스크립트 지원 : 조건식과 함수 사용
- 동적 모듈 로드 가능
- 그래픽 부트 메뉴
- ISO 이미지로 바로 부팅

```
nano /etc/grub.d/00_header
```

```
update-grub
```
grub 수정 후 변경 사항을 저장
