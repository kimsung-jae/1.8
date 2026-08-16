# 보글사다리 FILTER FINAL 1PICK V1.8

## 핵심
- 1차: 삼치기80 엔진이 4개 조합 중 위험도가 높다고 판단한 1개를 제외합니다.
- 2차: 남은 3개만 대상으로 Recent / Markov / Exact Shape / KNN 규칙을 동등 1표로 다시 비교합니다.
- 화면에는 실제 사용할 **최종 1픽 하나만 크게 표시**합니다.
- 1차 삼치기 적중률과 2차 최종 1픽 적중률을 분리합니다.
- 최종 1픽은 마지막 최대 30회를 미래값 가림 walk-forward로 재현해 적중률을 표시합니다.
- 배팅금액 기본 5,000원, 배당 기본 1.95. 최종 1픽의 실전 승패와 누적손익을 자동 기록합니다.
- 백그라운드 자동추첨 / JSON 백업·복원 / 실전성적 초기화 / 전체 초기화를 유지합니다.

> 주의: 1차 삼치기 80%가 2차 최종 1픽 80%를 뜻하지 않습니다. 1.95배라면 단일픽 손익분기 적중률은 약 51.3%입니다. 표시 적중률은 과거 순차 재현값이며 미래 적중을 보장하지 않습니다.

## GitHub Codespaces
```bash
bash 보글사다리_FILTER_FINAL1_V1.8_원클릭.sh
```

Actions > Build Android APK > Artifacts > `BubbleFilterBest1V18-debug-apk`

패키지: `com.bubbleladder.filterbest1v18`
