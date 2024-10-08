## 목차 ##
ⓐ [프로젝트 소개](#프로젝트-소개)
  1. [프로젝트 이름소개](#프로젝트-이름소개)
  2. [시연영상](#시연영상)
  3. [스토리보드](#스토리보드)


ⓑ [기술스택](#기술스택)
  1. [개발환경](#개발환경)
  2. [ERD 설계도](#erd-설계도)
  3. [기능설명](#기능설명서)


ⓒ [기술적 경험](#기술적-경험)

----------------------------------------------------------------------------------------------------

## 프로젝트 소개
### 프로젝트 이름소개
<img src="https://github.com/user-attachments/assets/3836f2b4-4ccf-441c-b2da-7b785585cb40" width="300px" height="200px"></br>

**코드브루란?**
<p>예약, 상품판매, 게시판 등의 서비스를 제공하는 커피숍의 홈페이지.</p>

-----------------------------------------------------------------------------------------------------

### 시연영상

[시연영상 링크](https://github.com/user-attachments/assets/dcb0f943-c146-4321-97ad-a90900f97d44)

------------------------------------------------------------------------------------------------------

### 스토리보드

**ⓐ 자유게시판**  
<img src="https://github.com/user-attachments/assets/38746db7-7a66-492e-bffb-6eb3279d1b00" width="45%" height="300px">
<img src="https://github.com/user-attachments/assets/1f2d1874-a044-4159-9f3e-bd2948b4d774" width="45%" height="300px">

**ⓑ 예약**  
<img src="https://github.com/user-attachments/assets/bfa93ebe-0cf4-4ae0-9fa6-b5465b9e6969" width="45%" height="300px">
<img src="https://github.com/user-attachments/assets/b2945b38-41d9-46fa-8579-d24398b3cd01" width="45%" height="300px">

**ⓒ 결제**  
<img src="https://github.com/user-attachments/assets/e6a3bfcf-18aa-42e1-97d2-c7050ef71ce2" width="45%" height="300px">

**ⓓ 회원**  
<img src="https://github.com/user-attachments/assets/94126a74-f0f7-49e1-937e-da69be4e4304" width="45%" height="300px">
<img src="https://github.com/user-attachments/assets/881208c1-0dc8-4e1d-819f-6dcab721d3cb" width="45%" height="300px">
<img src="https://github.com/user-attachments/assets/94c89910-ac99-4464-bbe4-6ed018ce5308" width="45%" height="300px">
<img src="https://github.com/user-attachments/assets/ad68dc70-1c7e-4577-9906-44cb2d228647" width="45%" height="300px">

**ⓔ 기타**  
<img src="https://github.com/user-attachments/assets/e1302bd5-f551-4624-8fb8-94a004000141" width="45%" height="300px">
<img src="https://github.com/user-attachments/assets/a94ec272-2fd8-4566-ade4-048f9b0e99b5" width="45%" height="300px">
<img src="https://github.com/user-attachments/assets/b7bf8f8e-f557-47c0-848a-14136030e974" width="45%" height="300px">
<img src="https://github.com/user-attachments/assets/b7bf8f8e-f557-47c0-848a-14136030e974" width="45%" height="300px">
<img src="https://github.com/user-attachments/assets/814c3132-2d9f-4549-bd34-bf13113ca31e" width="45%" height="300px">
<img src="https://github.com/user-attachments/assets/49a45f2d-de07-4d9c-8ce5-67a9981a69c3" width="45%" height="300px">
<img src="https://github.com/user-attachments/assets/e86c4e47-b764-42db-a03d-74ed3170933e" width="45%" height="300px">

------------------------------------------------------------------------------------------------------

## 기술스택

### 개발환경  
![개발환경](https://github.com/user-attachments/assets/7ae585f5-8cab-4925-b415-063bdf38793e)

### ERD 설계도  
![ERD 설계도](https://github.com/user-attachments/assets/5aa7c293-17db-4c58-a46f-f9f5699bb3ae)

### 기능설명서

1. 예약기능 (← 주로 맡은 부분)</br>
[예약기능 설명서 링크](https://adaptive-spike-72c.notion.site/750cae3810f344519ecee4f7d71e3eee?pvs=4)  

2. 결제기능 (← 주로 맡은 부분)</br>
[결제기능 설명서 링크](https://adaptive-spike-72c.notion.site/32f9ca588b314135a23dc93f77f99d20?pvs=4)   

3. 자유게시판 (← 일부 맡은 부분)</br>
[자유게시판 설명서 링크](https://adaptive-spike-72c.notion.site/0caf08619c7d4b53b00493a416dd33c3?pvs=4)    

4. 회원관련 (← 일부 맡은 부분)</br>
[회원관련 설명서 링크](https://adaptive-spike-72c.notion.site/f972baaf74f1458793e84e0bb0d0181c?pvs=4)    

------------------------------------------------------------------------------------------------------

## 기술적 경험

● 이미 예약된 좌석 비활성화하는 과정에서...  
프로젝트를 진행함에 있어 겪은 어려움:  
이 프로젝트에서는 사용자가 특정 날짜와 시간에 좌석을 예약할 때, 이미 예약된 좌석은 선택할 수 없도록 비활성화하는 기능을 구현하는데 있어 큰 어려움을 겪었습니다. 

● 해결 내용:

ⓐ 예약된 좌석 정보 가져오기:  
사용자가 날짜와 시간이 선택하는 두번째 슬라이드에서 비동기적으로 날짜(selectedDate), 시간(selectedTime) (+ 추가적으로 지점(branch))에 해당하는 예약된 좌석 정보를 모든 예약을 보는 쿼리문을 통해 DB에서 가져오게 하였습니다. 해당 지점과 시간대에 이미 예약된 좌석 정보를 JSON 형태로 받아옵니다. 

ⓑ 좌석 비활성화 로직:  
DB에서 받아온 예약된 좌석 목록은 함수로 전달되어, 페이지 상의 좌석 상태를 업데이트하게 하였습니다.  
먼저, 데이터에 없는 값은 기본값으로 설정되어 있던 모든 좌석의 `unavailable` 클래스를 제거한 후, 예약된 값은 `unavailable` 클래스를 추가했습니다.  
이렇게 하면 사용자가 이미 예약된 좌석을 선택할 수 없게 됩니다.

이를 통해 사용자는 실시간으로 예약 가능 여부를 확인하며, 중복 예약을 방지할 수 있었습니다.
