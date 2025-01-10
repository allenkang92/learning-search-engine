# 검색 엔진 개요

## 1. 검색 엔진이란?
- 컴퓨터 시스템에 저장된 정보를 찾아주는 정보 검색 시스템
- 검색 결과를 목록으로 표시
- 정보 검색 시간 최소화

## 2. 검색 시스템의 핵심 요구사항
- 빠르고 정확한 검색 결과 제공
- 사용자 경험 최적화
- 보안 및 개인정보 보호
- 확장성 및 유지보수의 용이성
- 상호 운영성 및 통합성

## 3. 검색 엔진의 기본 아키텍처
1. 데이터 수집 (크롤링)
2. 문서 정제 (비정형 → 정형)
3. 데이터 색인 (빠른 검색 가능 구조로 저장)
4. 검색 쿼리 처리

## 4. 검색 엔진 vs RDBMS

### RDBMS의 한계
- 전통적인 SQL 방식의 한계
- 복잡한 쿼리 문제
- 성능 이슈
- 사용자 의도 파악의 어려움

### 주요 차이점
1. 색인 방식
   - RDBMS: 컬럼 기준, ID 값 활용
   - 검색엔진: 필드 값을 Term 단위로 분해

2. 검색 방법
   - RDBMS: 전체 컬럼 정보 순차 비교
   - 검색엔진: 미리 정의된 색인 활용

3. 검색 대상
   - RDBMS: 구조화된 데이터
   - 검색엔진: 비정형 텍스트 포함

## 5. 검색 엔진의 품질 평가
### 주요 지표
1. 정확도(Precision)
   - 검색 결과 중 실제 원하는 문서의 비율
   - precision = number_retrieved_relevant / number_total_retrived

2. 재현율(Recall)
   - 가능한 모든 관련 문서 중 검색된 문서의 비율
   - recall = number_retrieved_relevant / number_possible_relevant

## 6. 주요 검색 엔진 종류
- Elasticsearch
- Splunk (로그 데이터 특화)
- OpenSearch
- Algolia
- MS Azure AI Search
