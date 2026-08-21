<div align="center">

# LMS 데이터 기반 학생 특성 분석 및 맞춤형 커리큘럼 추천

**학생 학습 행동 분석 · 통계적 검증 · 학생 그룹 분류 · 커리큘럼 제안**

<p>
  <img src="https://img.shields.io/badge/Statistics-Analysis-4C78A8?style=flat-square&logoColor=white">
  <img src="https://img.shields.io/badge/ANOVA-Statistical%20Test-5B8FF9?style=flat-square&logoColor=white">
  <img src="https://img.shields.io/badge/Tukey%20HSD-Post%20Hoc-61DDAA?style=flat-square&logoColor=white">
  <img src="https://img.shields.io/badge/Decision%20Tree-Student%20Profiling-F6BD16?style=flat-square&logoColor=white">
  <img src="https://img.shields.io/badge/Data%20Mining-Knowledge%20Discovery-9270CA?style=flat-square&logoColor=white">
</p>
<sub>🔐 실제 학생 데이터와 원본 연구 데이터는 개인정보 및 연구 데이터 보호를 위해 공개하지 않습니다.<br>
공개 가능한 범위에서 연구 목적, 데이터 구성, 분석 방법 및 주요 결과를 정리했습니다.</sub>

</div>

---

## 프로젝트 개요

LMS에 축적된 학생들의 학습 활동 데이터를 분석하여  
**학생별 학업 특성을 파악하고, 유사한 학습 패턴을 가진 학생들을 그룹화한 뒤  
각 그룹에 맞는 맞춤형 커리큘럼을 제안**한 연구 프로젝트입니다.

연구에서는 IT 관련 학과 학생의 LMS 활동 정보, 개설 강의 정보, 학생 학점, 강의계획서 데이터를 활용했습니다.

원천 데이터는 약 **2,000명 규모**였으며,  
데이터 정제 및 정규화 이후 **1,106명의 학생 데이터**를 분석에 활용했습니다. :contentReference[oaicite:2]{index=2} :contentReference[oaicite:3]{index=3}

> **LMS 데이터 → 특성 설계 → 통계적 검증 → 학생 그룹 분류 → 맞춤형 커리큘럼 제안**

---

## 연구 착안점

기존 수업 운영에서는 학생별 학업 특성과 수준을 일일이 파악하여  
수업 내용을 구성하거나 개별적인 케어를 제공하기 어려웠습니다.

이에 LMS에 축적된 학습 활동 데이터를 활용하여

- 학생들의 전반적인 학업 패턴 파악
- 유사한 학습 특성을 가진 학생 그룹 분류
- 그룹별 특성에 맞는 학습 지원 방향 제안

을 목표로 연구를 진행했습니다. :contentReference[oaicite:4]{index=4}

---

## 연구 데이터

| 데이터 | 활용 목적 |
|---|---|
| LMS 활동 로그 | 학생의 학습 활동 및 상호작용 분석 |
| 개설 강의 정보 | 수강 강의 및 강의 유형 분석 |
| 학생 학점 | 학업 성취 수준 분석 |
| 강의계획서 | 강의 방식 유형화 및 수강 특성 분석 |

### 학습 상호작용 변수

LMS 로그를 기반으로 학생의 학습 활동을 다음 4가지 유형으로 정의하고 계량화했습니다.

| 변수 | 의미 |
|---|---|
| Learner–Instructor | 학생–교수자 상호작용 |
| Learner–Learner | 학생–학생 상호작용 |
| Learner–Content | 학생–콘텐츠 상호작용 |
| Course Activities | 강의 및 LMS 활동 내역 |

강의계획서에서 정의된 유사한 강의 방식을 그룹화하여 다음 4가지 유형으로 분류했습니다. :contentReference[oaicite:5]{index=5}

- Lecture
- Practice / Experiment
- Flipped / Blended Learning
- Problem / Project Based Learning

---

## 분석 흐름

```text
LMS / Course / Grade / Syllabus Data
                │
                ▼
      Data Cleaning & Normalization
                │
                ▼
      Interaction Feature Engineering
                │
                ▼
       Exploratory Data Analysis
                │
                ▼
          ANOVA + Tukey HSD
                │
                ▼
        Decision Tree Modeling
                │
                ▼
       Student Group Profiling
                │
                ▼
    Personalized Curriculum Proposal
```
