### 석현 · Seokhyun
Software Developer | Android · Backend · AI

평택대학교 스마트콘텐츠학과 — 프로젝트를 직접 만들면서 문제를 찾고 해결하는 과정에 관심이 많습니다.

---

### Tech Stack

**Languages**
`Kotlin` `Java` `C++` `Python`

**Mobile**
`Android` `CameraX` `Google Maps SDK` `ViewModel · LiveData`

**Backend / Database**
`Spring Boot` `Kafka` `FastAPI` `Node.js` `Firebase` `PostgreSQL` `MySQL`

**AI / ML**
`PyTorch` `TensorFlow Lite` `MoveNet` `OpenAI API` `Claude API`

**Deploy**
`Render` `Linux`

**Tools**
`Git` `GitHub` `Android Studio` `VS Code`

---

### Featured Projects

**[SmartBulk](https://github.com/seokhyu-n/SmartBulk-app)**  
AI 기반 개인 맞춤 운동 추천 및 자세 피드백 Android 애플리케이션

Kotlin으로 개발한 Android 앱으로, TensorFlow Lite MoveNet을 이용한 온디바이스 자세 인식과 Firebase (Authentication / Realtime Database / Cloud Functions), Anthropic Claude API를 활용했습니다.

초기 수업 프로젝트에서는 자세 인식이 안정적으로 동작하지 않는 문제가 있었습니다. 처음에는 각도 임계값 문제로 판단했지만, 다시 분석해보니 카메라 프레임 회전 보정과 YUV 변환, TFLite 입력 처리 과정에 원인이 있었습니다. 이를 바탕으로 카메라/모델 추론과 운동별 판정 로직을 분리하고, 단일 임계값 대신 운동별 상태 머신 방식으로 구조를 다시 설계했습니다.

- 운동 종류별 자세 판정 로직 (10종)
- 연습 모드 / 날짜 기반 운동 계획 / 오늘의 운동 체크리스트
- Firebase Cloud Functions를 통한 AI 식단 추천 (API 키는 서버에서만 관리)

**[CVRP Road Demo](https://github.com/seokhyu-n/cvrp-road-demo)**  
차량 용량 제약이 있는 배송 경로 최적화(CVRP) 웹 데모

지도에 배송지를 입력하면 PyTorch 기반 모델(Transformer Encoder + Pointer 스타일 Decoder)이 방문 순서를 예측하고, 차량 용량 제약은 후처리 단계에서 검증하여 실제 운행 가능한 경로로 변환합니다. OSRM API로 실제 도로 기준 거리/시간을 계산하고 Leaflet으로 지도에 시각화합니다.

- FastAPI 백엔드 + PyTorch 기반 경로 예측 모델
- Kakao Local API / OpenStreetMap 지오코딩
- OSRM 실도로 라우팅, Leaflet 지도 시각화
- 초기 모델은 Baseline 대비 평균 −2.65%였지만, capacity-only repair + best-of-20 샘플링으로 **평균 +7.2% 개선**

**[RunBuddy](https://github.com/seokhyu-n/RunBuddy)** · 팀 프로젝트 (3명)  
실시간 러닝 트래킹 & AI 러닝 코치 Android 앱

GPS로 거리·페이스·칼로리·고도를 실시간 측정하고, 자연어로 요청하면 OpenAI가 러닝 코스를 추천해 지도에 표시합니다. AI API 연동(앱 ↔ Node.js AI 서버 ↔ OpenAI)과 러닝 중 지도 표시를 맡았습니다.

- API 키를 앱에 두지 않도록 AI 서버를 분리해 Render에 배포
- Google Maps Polyline 실시간 경로 시각화

**[BASISI](https://github.com/haakim7/Basisi)** · 팀 프로젝트 (5명)  
AI 데이터 분석 기반 베이비시터 검증·매칭 플랫폼

AI 및 메시징 처리를 맡아, 후기 등록 이벤트를 Kafka로 비동기 처리하는 파이프라인과 LLM 후기 감성 분석, 시터 활동 점수(불꽃 온도) 로직을 개발했습니다.

- Spring Boot · Kafka · LLM API(OpenAI · Gemini)

---

### Currently Learning

Backend Development · Database · Linux · Cloud · AI

---

### Certifications

- SQLD
- 리눅스마스터 2급
