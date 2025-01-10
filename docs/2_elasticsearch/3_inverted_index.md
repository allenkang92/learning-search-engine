# 역색인 (Inverted Index)

## 1. 개요
- Elasticsearch의 고성능 검색의 핵심 기술
- 빠른 검색을 가능하게 하는 데이터 구조

## 2. 작동 원리
### 전통적인 DB 검색
- 모든 문서 내용을 순차적으로 검색
- 키워드 포함 여부 확인
- 많은 연산 필요로 느린 속도

### 역색인 방식
- Term을 포함하는 문서에 대한 인덱스 테이블 생성
- 인덱스 테이블을 통한 빠른 검색
- 대량의 문서에서도 빠른 검색 가능

## 3. 특징
### 장점
- 빠른 검색 속도
- 대용량 데이터 처리 가능
- 검색 시스템에 최적화된 구조

### 단점
- 업데이트/삭제/삽입 시 큰 스토리지 오버헤드
- 높은 유지 관리 비용
- 자주 등장하는 단어 처리 시 성능 저하

## 4. 최적화 기법
### Stop Words
- 자주 등장하는 불필요한 단어 제거
- 예: 관사(a, the), 접속사(and), 조사 등
- 인덱스 크기 감소
- 검색 성능 향상