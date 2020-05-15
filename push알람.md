## Push 알람

- 공지사항 및 패치내용을 팝업 형태로 사용자에게 전달하기 위함

### 시나리오

1. ALPL 접속시 팝업이 바로 보여짐

- 패치내용일 경우 버전별로 history가 보여져야 할 것 같음
- 기간을 정해서 특정 기간동안의 패치내용만 보여지도록 함
- 공지사항이 필요할 경우, 한 popup에 tab으로 내용을 구분하도록 함
- 상단 아이콘(알림표시) 클릭으로 언제든 볼 수 있음

![](/img/img1.png)

### 구현방법

1. 웹소켓
2. serviceWorker:

https://developers.google.com/web/fundamentals/codelabs/push-notifications?hl=ko#%ED%95%84%EC%9A%94%ED%95%9C_%EC%82%AC%ED%95%AD

- 브라우저 알림 뜸 -> 클릭 -> 공지 popup출력

3. 첫 접속 시 팝업오픈, 이후엔 알림아이콘 클릭으로 오픈

- 클릭 시 최신내용 출력
