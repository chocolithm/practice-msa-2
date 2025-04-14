교재명 : 스프링으로 하는 마이크로서비스 구축 2E
학습기간 : 2025-04-09 ~


필요 설치사항
- JDK 16
- git, docker, curl, jq, spring, siege, helm, kubectl, minikube, istioctl


1장. 마이크로서비스 소개 2025-04-09
2장. 스프링 부트 소개 2025-04-09
3장. 공조 마이크로서비스 집합 생성 2025-04-10
4장. 도커를 사용한 마이크로서비스 배포 2025-04-10 ~ 2025-04-12
5장. OpenAPI를 사용한 API 문서화 2025-04-12
6장. 영속성 추가 2025-04-14
22장. 윈도우용 설치 지침 2025-04-10



기록사항
Docker
- docker는 레이어 분리를 통해 docker build 시 변경사항만 빌드하도록 구성

API
- 내부개발자용으로 openapi + swagger 활용 / tag, operation, apiResponse 등으로 상세 활용

공통모듈
- spring에서 서비스와 aop의 관계처럼, 마이크로서비스에서 공통모듈은 '단일 책임을 나누는 조력자'로서 역할 수행
- util, logging, security 등은 공통 모듈로 관리가 용이

MapStruct
- entity와 dto 변환을 처리해주는 라이브러리

Persistency
- delete는 멱등성을 지녀야 함 / 즉 데이터 삭제 여부와 무관하게 반환값이 같아야 함