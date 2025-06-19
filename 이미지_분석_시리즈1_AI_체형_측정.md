# 이미지 분석 시리즈 1편: AI는 사람의 체형을 얼마나 정확히 측정할 수 있을까?

> 사람의 체형을 AI가 얼마나 정확하게 분석할 수 있을까?  
> 직접 분석 도구를 만들어 실험한 과정을 기록합니다.

---

## AI 이미지 분석 – 가능한 작업 범주

ChatGPT를 기반으로 할 수 있는 이미지 분석 작업은 다음과 같습니다:

- **측정 및 좌표 분석:** 거리, 위치, 비율 계산 – 인물 키 예측 등
- **텍스트 추출:** 이미지 속 글자 인식 (OCR)
- **차트 해석:** 이미지 내 그래프나 표 인식
- **레이아웃 분석:** 디자인 피드백
- **요소 편집:** 배경 제거, 요소 추가 등
- **AI 이미지 생성:** 삽화, 도식 등 생성

---

## AI 기반 인물 분석 – 글로벌 연구 동향

AI가 얼굴, 신체 비율, 키, 포즈 등을 어떻게 분석하는지를 다룬 연구가 다수 존재합니다.

- **얼굴 황금비율:** Prokopakis et al. (2013), Pallett et al. (2010)
- **AI 얼굴 매력 분석:** Liu et al. (2019)
- **키 예측:** Günel et al. (CVPR 2018) – 평균 오차 약 5~6cm
- **자세 인식:** Zheng et al. 리뷰 (2020)

📚 **참고 출처:**  
[Cureus (2024)](https://www.cureus.com/articles/199834)  
[Günel et al. (CVPR 2018)](https://openaccess.thecvf.com/content_cvpr_2018/papers/Gunel_Estimation_of_Person_CVPR_2018_paper.pdf)  
[Liu et al. (2019)](https://arxiv.org/abs/1909.03605)

---

## 🧪 이번 시리즈에서 사용하는 AI 분석 도구 소개

AI가 할 수 있는 것과 사람이 최종 판단해야 할 것의 경계를 실험하며, 사람의 손에 의한 검증이 반드시 필요함을 느꼈고 이에 개발 경험이 전혀 없는 저는 ChatGPT의 도움을 받아서 두 가지 이미지 분석 도구를 만들었습니다.

이 도구들은 모두 ChatGPT와 연동된 이미지 기반 분석 툴이며, 클릭 기반 좌표 추출 → 자동 수치 계산 → 분석 → 평가로 이어지는 구조를 갖고 있습니다.

<img src="https://raw.githubusercontent.com/cbyun73/CBYun-Blog/main/Image_analysis_tool_sample1.png" width="60%">
<img src="https://raw.githubusercontent.com/cbyun73/CBYun-Blog/main/Image_analysis_tool_sample2.png" width="60%">