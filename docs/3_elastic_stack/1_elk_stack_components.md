# Elastic Stack (ELK Stack) 구성요소

## 1. Beats
### 데이터 수집기
- 다양한 데이터 소스로부터 실시간 데이터 수집
- Elasticsearch나 Logstash로 데이터 전송

### 주요 Beats 종류
- Filebeat: 로그 파일
- Metricbeat: 시스템 메트릭
- Packetbeat: 네트워크 데이터
- Heartbeat: 가용성 모니터링
- Winlogbeat: Windows 이벤트 로그

## 2. Logstash
### 데이터 처리 파이프라인
- 데이터 수집, 변환, 전송을 담당
- 플러그인 기반 아키텍처

### 주요 컴포넌트
1. Input
   - file: 파일 읽기
   - syslog: 시스템 로그 읽기
   - redis: Redis 데이터 읽기
   - beats: Beats 데이터 읽기

2. Filter
   - grok: 비정형 데이터 구조화
   - mutate: 필드 변경/추가/삭제
   - date: 날짜 형식 변환
   - gsub: 전처리 작업

3. Output
   - elasticsearch: ES로 데이터 전송
   - file: 파일로 저장
   - kafka: Kafka로 전송

### 특징
- 자체 메모리/파일 기반 큐
- 높은 처리 속도와 안정성
- 재시도 로직과 Dead-Letter-Queue 지원

## 3. Elasticsearch
### 핵심 검색/분석 엔진
- 데이터 저장, 검색, 분석
- RESTful API 제공
- 분산 시스템 아키텍처

## 4. Kibana
### 데이터 시각화 플랫폼
- Elasticsearch 데이터 시각화
- 실시간 모니터링
- 대시보드 제작

### 주요 기능
1. Discover
   - 데이터 탐색
   - 실시간 검색

2. Visualize
   - 차트 생성
   - 데이터 시각화

3. Dashboard
   - 여러 시각화 요소 통합
   - 실시간 모니터링

4. Settings
   - 인덱스 관리
   - 시스템 설정

## 5. Elastic Stack 특징
- 자동완성/필터/랭킹 기능
- 강력한 보안 기능
- 실시간 데이터 처리
- 확장 가능한 아키텍처
