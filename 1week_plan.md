# 📘 AWS 1주차 상세 학습 계획

## 🎯 목표

* AWS 기본 구조 이해
* 핵심 서비스 개념 숙지 (IAM, EC2, S3, RDS)
* 서비스 간 연결 구조 이해

---

## 📅 Day 1 — AWS 계정 생성 및 전체 구조 이해

### 학습 내용

* AWS 계정 생성
* Root 계정 vs IAM 계정
* Region / AZ 개념
* AWS 서비스 분류

### 실습

1. AWS 가입 및 로그인
2. 리전 변경
3. Billing Dashboard 확인

### 핵심 포인트

* AWS는 서비스 조합 플랫폼
* Region = 데이터센터 묶음

---

## 📅 Day 2 — IAM (권한 관리)

### 학습 내용

* IAM User / Group / Role / Policy
* 권한 구조 (Allow / Deny)

### 실습

1. IAM 사용자 생성
2. Admin 권한 부여
3. MFA 설정

### 핵심 포인트

* 보안의 시작은 IAM
* Root 계정 사용 최소화

---

## 📅 Day 3 — EC2 (가상 서버)

### 학습 내용

* EC2 개념
* Instance Type
* Key Pair / Security Group

### 실습

1. EC2 인스턴스 생성
2. SSH 접속
3. nginx 설치

```bash
sudo apt update
sudo apt install nginx -y
```

### 핵심 포인트

* EC2 = 클라우드 서버
* Security Group = 방화벽

---

## 📅 Day 4 — S3 (스토리지)

### 학습 내용

* Bucket / Object 구조
* Public vs Private

### 실습

1. S3 버킷 생성
2. 파일 업로드
3. Public 접근 설정

### 핵심 포인트

* S3 = 무제한 저장소

---

## 📅 Day 5 — RDS (데이터베이스)

### 학습 내용

* RDS 개념
* MySQL / PostgreSQL
* Endpoint

### 실습

1. RDS 생성
2. EC2에서 접속

```bash
mysql -h 엔드포인트 -u admin -p
```

### 핵심 포인트

* RDS = 관리형 DB

---

## 📅 Day 6 — 서비스 연결

### 학습 내용

* EC2 + S3 + RDS 구조
* 3-tier 구조

### 실습

* EC2 → S3 업로드

```bash
aws s3 cp test.txt s3://버킷명/
```

### 핵심 포인트

* AWS는 서비스 연결이 핵심

---

## 📅 Day 7 — 복습 및 미니 프로젝트

### 프로젝트 목표

* EC2 + S3 + RDS 연동

### 수행 내용

* 웹 서버 구축
* 이미지 저장
* DB 연결

---

## ✅ 최종 체크리스트

* [ ] IAM 이해
* [ ] EC2 생성 및 접속
* [ ] S3 업로드 및 접근
* [ ] RDS 연결
* [ ] 서비스 구조 이해

---

## 🔥 전략

* 단순 암기 금지
* 반드시 실습 중심
* 서비스 간 연결 이해

---

## 💡 확장 질문

1. EC2 대신 Lambda 사용 시 차이점은?
2. RDS vs DynamoDB 차이는?
3. S3 + CDN 구조는 어떻게 설계되는가?
