# AWS_WEB_HOSTING

Amazon S3 및 Route 53을 사용하여 AWS에서 정적 웹 사이트 호스팅

이 프로젝트는 Amazon S3를 사용하여 개인 웹 사이트를 설정하고 Amazon Route 53을 통해 사용자 지정 도메인과 연결하는 과정을 안내한다

### 1단계: 웹사이트 디자인
- 나만의 개인 웹사이트를 디자인하거나 기존 템플릿을 다운로드를 하자
- [free-css.com](http://free-css.com)에서 무료 템플릿을 확인 할 수 있다.

* 하지만 저의 경우 자체 제작했던 css, html을 사용했습니다.

### 2단계: Amazon S3 버킷 설정
- AWS Management Console로 이동하여 Amazon S3 콘솔로 이동
- '버킷 만들기'를 클릭하고 버킷의 고유한 이름을 입력
- '속성' 섹션에서 '정적 웹사이트 호스팅'을 활성화
- 웹사이트 파일을 버킷에 업로드
- 퍼블릭 액세스를 허용하도록 버킷 권한을 설정한다


![AWS_WEB1](https://github.com/plintAn/AWS_WEB_HOSTING/assets/124107186/212998ab-844f-4764-b4b2-0072b3749d0d)


### 3단계: Amazon Route 53을 통해 사용자 지정 도메인 구입
- Amazon Route 53 콘솔을 엽니다.
- '도메인 등록'을 선택한 다음 '도메인 등록'을 선택
- 안내에 따라 맞춤 도메인을 구매
- "Route 53 호스팅 영역"에서 새 레코드 세트를 생성
- S3 버킷의 엔드포인트를 별칭 대상으로 입력

구매한 도메인을 바탕으로 웹 페이지 배포 후 일정 시간 뒤 배포 확인

Output

https://www.plintan.com/
