# 손글씨 숫자 이미지 인식
## 프로젝트 동기
태블릿 손글씨 입력 기능을 사용하면서 글씨체가 다른 여러 손글씨들을 인식하는 기능에 흥미를 느꼈습니다.

마침 시연회 프로젝트를 만들시기가 되어 직접 손글씨를 인식할 수 있는 AI를 만들게 되었습니다.
## 프로젝트 설명
!!일부 코드만 공개되어 있습니다.

![image](https://github.com/SUNRINEmotion/7th-bomin_project/assets/141712723/17a4c4ba-893c-426c-a07d-66c9077c5ec5)

mnist 데이터셋을 활용하여 인공지능 모델을 만들었습니다.

mnist 데이터베이스는 손으로 쓴 숫자들로 이루어진 대형 데이터베이스입니다.

![image](https://github.com/SUNRINEmotion/7th-bomin_project/assets/141712723/6746aad3-9716-48a5-98bb-d12b6763d5fb)

X_train에는 60,000개의 픽셀 정보가 배열 형태로 저장되게 되고, Y_class_train에는 60,000개 이미지 정답인 클래스 정보가 담겨져 있습니다.

X_test와 Y_class_test는 테스트 데이터로 10,000개이고 형태는 위 학습데이터와 같습니다.

![image](https://github.com/SUNRINEmotion/7th-bomin_project/assets/141712723/0d154317-f8f1-4e43-b86d-edba3821679c)

학습을 위해 각 데이터를 0-255에서 0-1사이의 숫자로 변환합니다.

![image](https://github.com/SUNRINEmotion/7th-bomin_project/assets/141712723/5dc6de52-e3c1-4bc6-aeb8-44cf85031a87)

test를 진행할 데이터를 생성한 뒤, 모델을 실행시키면 됩니다.

![image](https://github.com/SUNRINEmotion/7th-bomin_project/assets/141712723/fadf6a53-8f3c-4a34-98e7-3081aa72d153)

6을 표현하기 위해 클래스 갯수를 가지는 리스트를 만들어 6번째 원소에만 1을 주는 방식으로 one-hot vector화 되어있습니다.

![image](https://github.com/SUNRINEmotion/7th-bomin_project/assets/141712723/3331ace9-092f-4cc0-8efe-b8efac8c5065)

원핫인코딩된 배열에서 1을 찾아 인덱스로 변환해주면 결과가 나옵니다.
## 결과 영상
[Uploading 녹음 2024-02-05 195625.zip…]()

## 개선 방안
숫자 말고 다른 글자로도 손글씨 인식을 하는 인공지능을 만들고 싶습니다.
