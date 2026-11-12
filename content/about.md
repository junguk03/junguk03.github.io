---
title: "About"
description: "웹 취약점 분석·모의해킹을 공부하는 정보보호학과 학생"
---

수원대학교 정보보호학과 학생입니다. **웹 취약점 분석과 모의해킹**을 목표로 공부하고 있습니다.
웹 서비스를 직접 만들어 본 경험을 바탕으로, 입력이 어디서 처리되고 어디서 검증이 빠지는지를 따라가며 취약점을 이해하려고 합니다.

## Education

- 수원대학교 지능형SW융합대학 정보보호학과 (2학년)

## 공부하는 방식

1. **PortSwigger Web Security Academy** 랩으로 취약점 유형을 익힌다
2. 같은 유형의 **워게임**(Dreamhack)을 풀며 익스플로잇 코드를 직접 짠다
3. 공개된 취약점을 **n-day로 재현**하고 원인과 대응까지 정리한다

글은 모두 직접 쓰고, 실패한 시도도 함께 기록합니다. 진행 상황은 [security_report](https://github.com/junguk03/security_report)에 있습니다.

## 다뤄 본 취약점

워게임·랩을 풀며 익스플로잇 코드를 직접 작성한 유형입니다. 코드는 [test_exploit_code](https://github.com/junguk03/test_exploit_code)에 있습니다.

| 분류 | 내용 |
| --- | --- |
| SQL / NoSQL Injection | Blind SQLi 자동화, MongoDB `$regex` 추출, CouchDB 특수 엔드포인트 조회, 객체 주입 인증 우회 |
| SSRF | 10진수 IP 표기로 필터 우회, 내부 포트 탐색 |
| Command Injection | 쿠키 값 `$(...)` 삽입, 결과 외부 전송 |
| Path Traversal → RCE | Tomcat 설정 파일 유출 → Manager로 WAR 웹셸 배포 |
| Authentication | IP 차단 우회, 에러 메시지·응답 시간 차이로 사용자명 열거 |
| Crypto | AES-CBC Padding Oracle Attack |

## 사용 기술

| 구분 | 기술 |
| --- | --- |
| Security | Burp Suite, Python (requests) |
| Backend | Python (Flask, FastAPI), Node.js (Express) |
| App | Flutter (GetX) |
| Infra | Docker, Redis, Linux, GitHub Pages |

## Links

- GitHub — [github.com/junguk03](https://github.com/junguk03)
- Naver Blog — [blog.naver.com/junkuk9503](https://blog.naver.com/junkuk9503)
