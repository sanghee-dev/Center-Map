# Center Map🗺️
지도에서 N개의 위치가 주어졌을 때 중간 위치를 지도해 표시해주는 서비스입니다.

## 스킬
- Swift
- MVC Pattern
- MapKit


## 기술 블로그
[기술 블로그 링크](https://velog.io/@leeesangheee/Center-Map-%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8)

## 기존 깃허브
[기존 깃허브 링크](https://github.com/della-padula/YappUltraHardPractice/tree/personal/Sanghee-2/Sanghee/Practice2/Practice2)


## 특징

### 요구사항
- 코드베이스 오토레이아웃을 사용합니다.
- MapKit 사용합니다.
- 중간 위치 계산하는 모듈 별도 설계합니다(Singleton 패턴 사용).
- 중간 위치 계산 후에 추가된 위치 좌표가 모두 화면에 들어오도록 Zoom-Out 혹은 Zoom-In 처리합니다.

### 위치 추가 방법
- 최대 개수는 10개입니다.
- 지도에서 특정 위치를 길게 터치시 Alert를 띄웁니다.
- 위치가 추가될 때마다 중간 위치를 계산해 중간 위치를 수정합니다.
- 추가된 위치와 중간 위치 모두 마커로 표시하며 색은 모두 다르게 지정합니다.

### 위치 제거 방법
- 추가된 위치 마커를 터치시 Alert를 표시합니다.
- 삭제할 때마다 중간 위치를 계산해 중간 위치를 수정합니다.
- 위치 마커가 하나 이하일 경우 중간 위치 마커도 사라집니다.

## 화면

### 시작 화면
- 위치를 요청한 이후 유저의 위치를 기준으로 지도를 확대합니다.
<img src="https://user-images.githubusercontent.com/61302874/135650630-83e2b068-2612-4cce-8eb8-d7fa45b199ae.gif" width="300" align="left" >
<img src="https://user-images.githubusercontent.com/61302874/135650677-a8574ee1-c387-443f-ad2a-a61037ce2385.gif" width="300" >

### 위치 추가
- 지도에서 특정 위치를 길게 터치시 Alert를 띄웁니다.
- 예를 선택하면 해당 위치에 마커를 추가합니다.
<img src="https://user-images.githubusercontent.com/61302874/135650739-84d1511f-60bb-4586-b887-ce2e222af2e8.gif" width="300" >

### 중앙 마커
- 위치가 2개 이상일 시에 중간 거리를 계산하여 마커가 표시됩니다.
- 위치가 추가되면 중앙 거리를 다시 계산해 중앙 마커를 수정합니다.
<img src="https://user-images.githubusercontent.com/61302874/135650803-693e11f3-1af0-4e59-9d14-ed48f0751e4b.gif" width="300" >

### 위치 삭제
- 마커를 터치시 Alert를 띄웁니다.
- 예를 선택하면 마커가 삭제됩니다.
- 마커가 삭제되면 중앙 거리를 다시 계산해 중앙 마커를 수정합니다.
<img src="https://user-images.githubusercontent.com/61302874/135650870-93e5088a-eb18-4f06-a7f5-5f5312926030.gif" width="300" align="left" >
<img src="https://user-images.githubusercontent.com/61302874/135650922-49dd0281-7e00-4865-9c50-3b9b87ab69e8.gif" width="300" >
