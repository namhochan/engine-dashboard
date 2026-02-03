# engine-dashboard
뉴스리서치 
⚠️ YOUR_ID 와 engine-dashboard 만 너 repo에 맞게 수정

# 📊 Engine Dashboard

엔진 분석 결과를 **자동 수집·정리하여 시각화하는 GitHub 기반 대시보드**입니다.  
서버 크론 의존도를 줄이고, GitHub Actions + Pages를 활용해  
리서치·분석 현황을 안정적으로 제공합니다.

---

## 🔍 이 대시보드는 무엇을 하나요?

- 시장 리스크 레벨 요약
- 테마 강도 및 트리거 카운터
- 최신 엔진 분석 결과 스냅샷
- 주요 종목/섹터 상태 요약
- 일별 자동 갱신 데이터 표시

👉 모든 화면은 **엔진 출력 JSON 데이터**를 기준으로 자동 반영됩니다.

---

## 🚀 라이브 대시보드
👉 **Dashboard 바로가기**  
https://YOUR_ID.github.io/engine-dashboard/

(정해진 시간에 자동 업데이트)

---

## 🧠 시스템 구성 흐름



[Engine 분석]
↓
[JSON 데이터 생성]
↓
[GitHub Actions 자동 실행]
↓
[data/latest.json 업데이트]
↓
[GitHub Pages 대시보드 반영]


---

## 📁 프로젝트 구조



engine-dashboard/
├─ dashboard/ # 대시보드 UI (웹)
├─ data/ # 엔진 결과 데이터
│ └─ latest.json
├─ .github/
│ └─ workflows/ # 자동 실행 / 배포
└─ README.md


---

## ⏱ 자동 업데이트 방식

- GitHub Actions 스케줄 실행
- 엔진 스크립트로 최신 데이터 생성
- JSON 파일 커밋
- GitHub Pages 자동 반영

👉 서버 크론 부담을 최소화한 구조입니다.

---

## 📌 사용 목적

- 엔진 분석 결과 **한 눈에 파악**
- 리서치 상태 / 트리거 흐름 추적
- 자동 리포트 기반 판단 보조
- 대시보드 중심 운영 구조 전환

---

## ⚠️ 참고 사항

- 실시간 스트리밍이 아닌 **주기적 스냅샷 대시보드**
- 데이터 정확성은 엔진 출력에 의존
- UI 및 분석 항목은 확장 가능

---

## 📅 최근 데이터
- 최신 기준 시각: `data/latest.json` 참고
