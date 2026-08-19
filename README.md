### 서석현 · Seokhyun
Software Developer | Android · Backend · AI

평택대학교 스마트콘텐츠학과 — 프로젝트를 직접 만들면서 문제를 찾고 해결하는 과정에 관심이 많습니다.

---

### Tech Stack

**Languages**
`Kotlin` `Java` `C++` `Python`

**Backend / Database**
`Firebase` `MySQL`

**AI / ML**
`TensorFlow Lite` `MoveNet`

**Tools**
`Git` `GitHub` `Android Studio` `VS Code`

---

### Featured Projects

**[SmartBulk](https://github.com/seokhyu-n/SmartBulk-app)**
AI 기반 개인 맞춤 운동 추천 및 자세 피드백 Android 애플리케이션

Kotlin으로 개발한 Android 앱으로, TensorFlow Lite MoveNet을 이용한 온디바이스 자세 인식과 Firebase(Auth / Realtime Database / Cloud Functions), Anthropic Claude API를 함께 사용했습니다.

초기 수업 프로젝트에서는 자세 인식이 안정적으로 동작하지 않는 문제가 있었습니다. 처음엔 각도 임계값 문제로 판단했지만, 다시 분석해보니 카메라 프레임 회전 보정과 YUV 변환, TFLite 입력 처리 과정에 원인이 있었습니다. 이를 바탕으로 카메라/모델 추론과 운동별 판정 로직을 분리하고, 단일 임계값 대신 운동별 상태 머신 방식으로 구조를 다시 설계했습니다.

- 운동 종류별 자세 판정 로직 (10종)
- 연습 모드 / 날짜 기반 운동 계획 / 오늘의 운동 체크리스트
- Firebase Cloud Functions를 통한 AI 식단 추천 (API 키는 서버에서만 관리)

**[CVRP Road Demo](https://github.com/seokhyu-n/cvrp-road-demo)**
차량 용량 제약이 있는 배송 경로 최적화(CVRP) 문제를 AI로 풀어보는 웹 데모

지도에 배송지를 찍으면 PyTorch 기반 모델(Transformer Encoder + Pointer 스타일 Decoder)이 방문 순서를 예측합니다. 모델 예측에만 전적으로 의존하지 않고, 차량 용량을 초과하는 시점만 프로그램적으로 판단해 출발지 복귀 지점을 삽입하는 방식으로 실제로 쓸 수 있는 경로를 만들었습니다. OSRM API로 실제 도로 기준 거리/시간을 계산하고 Leaflet으로 지도에 시각화합니다.

- FastAPI 백엔드 + PyTorch 기반 경로 예측 모델
- Kakao Local API / OpenStreetMap 지오코딩
- OSRM 실도로 라우팅, Leaflet 지도 시각화

---

### Currently Learning

Backend Development · Database · Linux · Cloud · AI

---

### Certifications

- SQLD
- 리눅스마스터 2급
