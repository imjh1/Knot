# knot

음성 인식 노트 필기 어플리케이션

## 프로젝트 제안 배경
음성 인식 기능(STT)를 탑재하여 청각장애인이 활용 가능한 노트 필기 앱 제작
음성을 녹음할 수 있기 때문에 사용자는 꼭 필요한 필기만 작성할 수 있으며 필요시 녹음한 음성, STT와 동기화된 자신의 필기를 재생하면서 추가적으로 필기가 가능합니다.

## 전체 구조
![구조도](https://user-images.githubusercontent.com/91405382/210517327-6c5d534a-3400-409d-ac2b-9ccb2e69c067.jpg)

## 결과물: 구현 화면

### 오디오 및 녹음 필기
노트 화면에서 드래그를 통해 필기를 하고 더블 탭을 통하여 필기를 지울 수 있다. 노트화면에서 상단의 빨간 버튼을 눌러 오디오 녹음을 시작한다. 이 때 노트를 필기하면 이후에 오디오와 동기화하여 재생할 수 있다. 또한 현재 필기하고 있는 화면을 스크린샷을 찍어서 thumbnail로 만들어 사용한다.

![쿠모쿠모노트필기](https://user-images.githubusercontent.com/91405382/210518153-3f7ab15f-6c9f-4e8c-8d24-477f10b07efb.gif)
![쿠모쿠모썸네일](https://user-images.githubusercontent.com/91405382/210518234-9088d218-d5d7-4cc5-8835-a79bd8713bc2.gif)

### 오디오 및 노트 재생
녹음 시작 시간 및 종료 시간으로 노트 파일이 저장된다. 상단의 회색 바를 누르면 저장된 오디오가 필기한 내용이 동기화 되어 재생된다.

![쿠모쿠모노트재생](https://user-images.githubusercontent.com/91405382/210518471-85880bb6-62ec-4955-916f-9c81d7073560.gif)

### 노트 스크롤
오디오 파일은 상단의 회색 바에 선택 가능하도록 나열된다. 회색 바를 스크롤하여 선택 재생 가능하다.

![쿠모쿠모음성스크롤](https://user-images.githubusercontent.com/91405382/210518615-296c9a97-8de3-4e28-aec4-d645c0ca2de0.gif)

### Speech to text로 오디오를 텍스트로 변환
마이크 입력으로 들어오는 오디오를 텍스트로 변환하여 화면에 표시한다. (iPhone XR – 한글 STT)

![쿠모쿠모음성인식](https://user-images.githubusercontent.com/91405382/210518777-7d8c5fb3-a250-4cc2-a79e-b63d5330ca06.gif)

### 변환된 텍스트 위에 노트 필기
텍스트 위에 노트 필기가 가능하며 스크롤로 화면이 이동하여도 노트는 텍스트와 함께 위치한다. (Pixel XR – 영어 STT)

![쿠모쿠모음성인식스크롤](https://user-images.githubusercontent.com/91405382/210518948-5a7f70f5-9b09-471b-ae03-6650c50b56e1.gif)

### 서버를 이용하여 기기간 동기화
메인 화면에서 업로드 버튼을 누르면 노트 파일이 서버에 저장된다. 이후 다운로드 버튼을 통해 서버의 노트 파일을 불러 기기간 동기화를 할 수 있다. (좌 iPhone, 우 Pixel XR)

![쿠모쿠모노트동기화](https://user-images.githubusercontent.com/91405382/210519127-87b7e254-9f0e-42e4-aa95-073bd94cc769.gif)

### 이미지를 삽입하여 그 위에 필기
노트 화면에서 사진첩 버튼을 누르면 갤러리에 접근하여 이미지를 불러올 수 있다. 이 때 스크롤로 화면을 이동해도 노트는 사진 위에 남아있다.

![쿠모쿠모이미지삽입](https://user-images.githubusercontent.com/91405382/210519299-96fa69c2-d8c9-4aa9-a8a5-95e6beb19509.gif)

### 이미지 동기화
이미지 또한 노트 파일에 포함시켜 기기간 동기화가 가능하다. (좌 iPhone, 우 Pixel XR)

![쿠모쿠모이미지동기화](https://user-images.githubusercontent.com/91405382/210519383-ba902a07-41e8-4474-abe4-b8d7c87bd181.gif)

### 크기가 다른 화면에서 입력된 필기간의 호환성
우측(iPad 11inch), 좌측(iPhone XR)간에 필기가 호환되는 것을 확인할 수 있다.

![쿠모쿠모가로길이](https://user-images.githubusercontent.com/91405382/210519484-47c35aac-d539-4301-bb93-9fdcbdcf1ea8.gif)



