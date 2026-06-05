# Sub-study 기획: Uptake 중 자연 호흡 패턴과 FDG SUVR 매개 분석

**작성일:** 2026-06-05  
**상태:** 아이디어 검토 완료, 설계 방향 확정 전  
**연계 연구:** RSP_PET V1.0 (IRB 승인, 데이터 수집 전)

---

## 1. 아이디어 출발점

FDG PET 촬영 시, **주입 후 30분 uptake 기간이 실제 뇌 대사 상태를 결정**한다.  
이 30분 동안 피험자가 어떻게 호흡하느냐에 따라 FDG 분포가 달라질 수 있음.

**핵심 질문:**
> 석문호흡 전문가는 uptake 중 자연 호흡 패턴 자체가 다른가?  
> 그리고 그 호흡 패턴 차이가 FDG SUVR 차이를 매개하는가?

---

## 2. V1.0 대비 달라지는 것

| | V1.0 메인 연구 | 이 Sub-study |
|--|--------------|-------------|
| 답하는 질문 | 장기 훈련이 뇌 대사를 바꿨나? (Trait) | 훈련이 자연 호흡 State를 바꾸고, 그게 SUVR을 매개하는가? |
| 추가 PET | 없음 | 없음 |
| IRB 변경 | 없음 | 없음 (비침습적 측정 추가) |
| 추가 측정 | — | 호흡 벨트 + capnography (uptake 30분) |

---

## 3. 왜 "forced deep breathing"보다 이 설계가 더 강한가

강제로 deep breathing을 시키면 **"지시에 따른 반응"** 을 보게 됨.  
반면, **지시 없이 자연스럽게 다른 호흡**이 나타난다면:

```
Trait (장기 훈련) → 자연 호흡 State로 발현 → SUVR 차이
```

이게 증명되면 인과 경로가 훨씬 명확해짐.  
또한 시키지 않은 행동이므로 ecological validity가 높음.

---

## 4. 논문 방향 — 신경과학 (Angle 1 + C 결합)

### 1차 분석: Mediation Analysis
```
Expert status → 호흡 파라미터 변화 → FDG SUVR 차이
(Independent)     (Mediator)            (Outcome)
```

### 2차 분석: Regional Specificity
- 호흡-SUVR 매개 효과가 **어느 뇌 영역에서 특이적으로 나타나는가**
- 글림패틱 가설 기반 ROI: PCC, Precuneus, Hippocampus, Entorhinal cortex

### 논문 스토리 구조

```
Introduction
  └─ 글림패틱 기능 ← 호흡이 driving force (Lim 2025 등)
  └─ FDG PET ← 글림패틱 기능의 간접 지표
  └─ 공백: uptake 중 호흡 패턴이 SUVR에 미치는 영향 미연구
  └─ 석문호흡 전문가 = 이 메커니즘 탐색의 이상적 모델

Methods
  └─ V1.0 프로토콜 + uptake 중 호흡 벨트 + capnography
  └─ 호흡 파라미터 추출 (RR, 깊이, 규칙성, I:E ratio)
  └─ FDG SUVR mediation analysis
  └─ Region-specific analysis (atlas-based ROI)

Results
  └─ 전문가, uptake 중 자연 호흡이 다름 (RR↓, 깊이↑, 규칙성↑)
  └─ 이 호흡 차이가 SUVR 차이를 부분 매개
  └─ 효과는 PCC, precuneus, hippocampus에서 특이적

Discussion
  └─ 훈련 → Trait → 자연 호흡 State로 발현
  └─ → 글림패틱 관련 영역 대사 보존
  └─ → PET 연구에서 uptake 중 호흡 통제 필요성 제기
```

---

## 5. 추가로 수집해야 할 데이터

| 측정 항목 | 장비 | 목적 |
|----------|------|------|
| 호흡 신호 | 호흡 벨트 (respiratory belt) | RR, 깊이 proxy, I:E ratio, 규칙성 |
| EtCO₂ | Capnography | CO₂ confound 통제 (필수) |

**수집 시점:** FDG 주입 직후 ~ 촬영 시작 전 30분 전 구간

---

## 6. 추출할 호흡 파라미터

| 파라미터 | 의미 |
|---------|------|
| RR (breaths/min) | 호흡 속도 |
| 진폭 평균 (belt amplitude) | 호흡 깊이 proxy |
| CV of RR | 호흡 규칙성 (낮을수록 규칙적) |
| I:E ratio | 흡기:호기 비율 |
| EtCO₂ | 이산화탄소 분압 (confound 통제용) |

---

## 7. 연구 공백 지도

```
알려진 것
├── FDG SUVR은 노화·AD에서 달라짐
├── 호흡이 뇌혈류를 급성으로 바꿈 (fMRI)
├── 명상/요가 수련자는 뇌 구조가 다름 (VBM)
└── CSF 흐름은 호흡에 의해 변함 (PC-MRI, Lim 2025)

모르는 것 ← 논문이 들어갈 자리
├── ❌ Uptake 중 자연 호흡이 FDG SUVR에 얼마나 영향 주는가?
├── ❌ 장기 훈련자는 uptake 중 자연 호흡 패턴이 다른가?
├── ❌ 호흡 패턴이 전문가-대조군 SUVR 차이를 매개하는가?
└── ❌ 이 효과는 글림패틱 관련 영역에서 특이적인가?
```

---

## 8. 리뷰어가 지적할 약점 + 방어 전략

| 약점 | 방어 전략 |
|------|---------|
| CO₂ confound: 깊은 호흡 → 혈관 수축 → FDG 전달 감소 | Capnography로 EtCO₂ 측정 → 공변량으로 통제 |
| 소뇌 기준 영역 타당성: 호흡이 소뇌 대사도 바꿀 수 있음 | Pons 등 alternative reference region 병용, sensitivity analysis |
| 30분 평균의 한계: 초반/후반 호흡 패턴 다를 수 있음 | 신호를 10분 단위로 나눠 안정성 검증 |
| Mediation N 부족: 각 군 30명 빠듯 | 탐색적 분석으로 프레이밍, effect size CI 보고 |

---

## 9. 교수님 설득 전략

### 지도교수님 (State vs Trait 딜레마 해결)
- 현재 연구의 핵심 약점: "훈련 효과인지 일시적 개입인지 모호"
- 이 sub-study가 직접 보완: Trait가 자연 State로 발현되는 경로 증명
- 추가 비용: 호흡 벨트 + capnography만 (PET 추가 없음, IRB 재심 없음)

### 핵의학과 협력교수님 (방법론적 기여)
- Uptake 중 호흡이 SUVR에 미치는 영향 — 아직 체계적 연구 없음
- 이 집단(호흡 전문가)으로 처음 보임
- NeuroImage / J Cereb Blood Flow Metab 급 투고 가능

---

## 10. 타겟 저널

| 저널 | IF | 적합 이유 |
|------|----|---------|
| NeuroImage | ~5-6 | 신경영상 + 방법론 기여 |
| Human Brain Mapping | ~4-5 | 뇌-행동 관계 연구 |
| Journal of Cerebral Blood Flow & Metabolism | ~6 | 대사 + 혈류 연결 |

---

## 11. 다음 단계

- [ ] 호흡 벨트 uptake 구간 기록 여부 프로토콜에 명시
- [ ] Capnography 장비 확보 가능 여부 핵의학과 협의
- [ ] Mediation analysis 방법론 검토 (causal mediation vs Baron-Kenny)
- [ ] V1.0 분석 파이프라인에 호흡 파라미터 추출 코드 추가 계획
