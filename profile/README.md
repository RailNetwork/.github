# RailNetwork

> 철도에 대해 알고 싶었던 정보를 한 눈에.

크로스플랫폼을 지원하는 철도 정보 어플리케이션입니다.

[공식 홈페이지](https://railnetwork.kr/)

## 기여자

### 2p31-1

- [GitHub](https://github.com/2p31-1)
- Flutter 프론트엔드 개발 전담 (AOS, iOS 크로스플랫폼)
- 알고리즘 기획
- 각종 데이터 정제 Python 스크립트 작성

### hjs0410hc

- [GitHub](https://github.com/hjs0410hc)
- Express 백엔드 개발 전담
- Oracle Cloud 인프라 구성 및 관리 (Linux+Nginx)
- CI/CD 구축 (Jenkins)

## 기능

<details>
  <summary>프론트엔드</summary>

</details>

<details>
  <summary>백엔드</summary>

- REST API 제공
- 공공 API를 호출하고 출력 데이터에 대해 자체 알고리즘을 수행하여 각 열차의 지연시간 계산 후 업데이트
- 열차의 편성번호에 대해 사용자의 의견을 수렴하여 정보 업데이트
- 데이터베이스에 열차 운행정보 저장

</details>

## 이렇게 개발했습니다

### 데이터 정제 자동화

수도권 전철의 다양한 데이터 형식에 맞게 각각의 변환 엔진을 만들어 엑셀 파일을 서버에서 사용할 수 있는 데이터인 `JSON`로 정제합니다.

![convertengines](imgs/convertengines.png)

### 다이어그램 활용

굳이 코드를 하나하나 읽지 않아도, 자체 알고리즘의 로직을 한 눈에 이해하기 쉽도록 `mermaid` 다이어그램으로 관리했습니다. =

![diagram1](imgs/diagram1.png)

![diagram2](imgs/diagram2.png)

### 리팩토링

최대한 코드의 가독성을 높이기 위해 다이어그램에서의 분기를 토대로 코드를 분리하고, 각각의 함수가 각각의 책임을 가질 수 있도록 개발했습니다.

![functions](imgs/functions.png)
