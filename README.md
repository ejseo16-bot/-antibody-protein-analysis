# -antibody-protein-analysis
# Antibody Protein Mass Distribution Analysis

## 분석 목적
UniProt 공개 데이터를 활용하여 사람(Human) 항체 관련 단백질의
분자량 분포와 구조적 특성을 탐색적으로 분석하였습니다.

## 사용 데이터
- 출처: UniProt REST API (reviewed human antibody proteins)
- 규모: 187개 단백질, 5개 변수 (ID, 이름, 길이, 분자량, 유전자명)

## 주요 결과
- 평균 분자량: 36,842 Da (중앙값: 28,710 Da)
- 분자량 분포는 오른쪽 꼬리를 가진 비대칭 분포
- IgM(IGHM)이 143,680 Da로 가장 큰 항체 사슬로 확인
- 아미노산 길이와 분자량 간 강한 선형 상관관계 확인 (≈110 Da/aa)

## 사용 기술
Python · pandas · matplotlib · UniProt REST API

## 파일 구성
- antibody_analysis.ipynb : 전체 분석 노트북
- antibody_proteins.csv : 정제된 데이터
- antibody_analysis.png : 시각화 결과
