# Fit-Got-U

최근 홈 트레이닝에 대한 수요가 증가하고 있다. 수 많은 홈 트레이닝 관련 어플리케이션이 존재하지만 가장 큰 문제점은 운동에 대한 설명과 방법이 충분한 것에 비해, 운동을 하는 당사자가 운동이 정확한 지 알기 힘들고 운동에 대한 피드백은 적다는 것이다. 
또한, 일반적으로 운동을 하는 사람들은 잘못된 운동 자세로 신체에 무리를 줄 수 있다. 우리는 이 문제점을 Pose Estimation을 통해 사람의 움직임을 실시간으로 보여주는 것과 음성 피드백으로 해결하고자 했다. 이를 통해, 많은 사람들에게 좀 더 정확하고 편한 홈 트레이닝과 많은 금전적을 비용을 들이지 않아도 누구나 언제 어디서든 운동을 할 수 있는 충분한 기회를 제공하고자 한다. 


> ### 1. Environment

	Android Studio 3.4

	Android SDK 28
	Android NDK 16
	Python3
	TensorFlow(1.4)
	MACE(0.9.0, mac os 10.x이상 필요)
	OpenCV 3.4.1
	삼성 갤럭시 s9+(SM-G965x) - Android Version 8(Oreo)
	NodeJS 8
	JAVA 8
	AWS EC2
	Apache 2.4
	MYSQL 5.5
	PHP 7.2
	Firebase SDK 17
	KAKAO SDK 1.17.0











json 형식 내의 좌표 정보 순서는 다음과 같다.
TOP, NECK, R_SHOULDER, R_ELBOW, R_WRIST, L_SHOULDER< L_ELBOW, L_WRITST, R_HIP, R_KNEE, R_ANKLE, L_HIP, L_KNEE, L_ANKLE 로 총 14개의 KeyPoint

2019-05-02 카메라 전면부로 수정
2019-05-07 간단한 선택 UI 추가. PoseEstiamtion화면에 선택한 운동과 종료버튼 추가(다시 스켈레톤 보이게, sleep 500ms)
2019-05-12 스쿼트 피드백 1차
2019-05-17 스쿼트 피드백 2차
2019-05-20 스쿼트 피드백 3차, 운동에 대한 음성 피드백 작성중(TTS 실패 다른 방법)
2019-05-28 런지 각도 및 피드백 추가 1차
2019-05-30 MediaPlayer로 음성 파일 추가, 재생은 되지만 쓰레드 문제로 전부 재생되지는 않는 오류
2019-06-03 런지 피드백 및 실루엣
2019-06-10 음성 피드백을 위해 AsyncTask사용
2019-06-11 테스트 시작(최적화)
