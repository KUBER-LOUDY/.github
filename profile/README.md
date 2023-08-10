# Kuber-Loudy 
기간 : 2023.06.30~2023.08.11

<img src="https://img.shields.io/badge/springboot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white"> <img src="https://img.shields.io/badge/next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white"> <img src="https://img.shields.io/badge/react-61DAFB?style=for-the-badge&logo=react&logoColor=black"> <img src="https://img.shields.io/badge/oracle-F80000?style=for-the-badge&logo=oracle&logoColor=white"> <img src="https://img.shields.io/badge/amazonaws-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white">  <img src="https://img.shields.io/badge/mysql-4479A1?style=for-the-badge&logo=mysql&logoColor=white"> <img src="https://img.shields.io/badge/javascript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black"> <img src="https://img.shields.io/badge/html5-E34F26?style=for-the-badge&logo=html5&logoColor=white"> <img src="https://img.shields.io/badge/python-3776AB?style=for-the-badge&logo=python&logoColor=white"> <img src= "https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white"> <img src="https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white"> <img src ="https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white">

[@mantech-om](https://github.com/mantech-om) 의 [제 5회 오픈인프라 경진대회](https://www.oidc.co.kr) 본선 진출작입니다.

## 1. About
**Kuber-Loudy**는 **버튼 하나로 시작하는 쿠버네티스 어플리케이션 API 도우미** 입니다. 클라우드 공급업체의 **가장 경량급 서버**만을 이용하여, 클라우드 컨테이너 환경을 시작하게 도와줍니다. 사용자의 AWS IAM 계정을 받아, EC2 생성 및 K8s 연결을 K8s API에 기반하여 자동으로 구현합니다.

![image](https://github.com/KUBER-LOUDY/.github/assets/77730511/45a8ed38-c84e-455f-b4da-ca536fa51649)

## 2. Infomation

### system
<img width="772" alt="image" src="https://github.com/KUBER-LOUDY/.github/assets/77730511/bc6daa1d-7ffa-4286-a689-5cfeb757e5b5">

### Installation
1. [백엔드 레포 다운](https://github.com/KUBER-LOUDY/kuber-loudy-spring-boot)
2. IntelliJ 에서 아래 폴더 구조에 yml 및 config 파일 추가

<details>
<summary>백엔드 폴더 구조 config</summary>
<div markdown="1">

```bash
.
├── LICENSE
├── README.md
├── build.gradle
├── kl-admin
│   ├── build.gradle
│   └── src
│       └── main
│           ├── java
│           └── resources
│               └── **application-admin.yml**
├── kl-api
│   ├── build.gradle
│   └── src
│       ├── main
│       │   ├── java
│       │   └── resources
│       │       └── **application.yaml**
├── kl-common
│   ├── build.gradle
│   └── src
│       └── main
│           ├── java
│           └── resources
│               ├── **apllication-common.yml**
│               ├── awsconfig
│               │   ├── **config**
│               └── ociConfig
│                   ├── **{oci pem key}**
│                   └── **config**
├── kl-domain
│   ├── build.gradle
│   └── src
│       └── main
│           ├── java
│           └── resources
│               ├── **application-domain.yml**
│               ├── **config**
│               └── **kl2bastion_rsa**
└── settings.gradle
```


</div>
</details>

3. spring project 실행
4. [프론트 레포 다운](https://github.com/KUBER-LOUDY/kuber-loudy-front)
5. VScode 에서 프론트 레포 다운 후 차례로 실행
```bash
npm install
npm run dev
```

### WiKi
레포지토리 별 코드 설명 및 참고는 아래 위키 링크를 참고해 주십시오.
- [spring-boot-server](https://github.com/KUBER-LOUDY/kuber-loudy-spring-boot/wiki)


## 3. Demo Video & ScreenShots

### Video

https://github.com/KUBER-LOUDY/.github/assets/77730511/6b5089ad-2579-4fe5-97f8-0f6631458797

### Screen Shots
<img width="1512" alt="image" src="https://github.com/KUBER-LOUDY/.github/assets/77730511/599ee14f-f591-4221-b44c-af3ff034b51f">
<img width="1512" alt="image" src="https://github.com/KUBER-LOUDY/.github/assets/77730511/41a02c00-f77f-498f-a7bb-d7bb24a5f654">

## 4. Contributors
<table border="1" cellspacing="0" cellpadding="0" width="90%">
    <tr width="100%">
        <td width="20%" align="center"><a href= "https://github.com/yhjune">Hyojung Yoon</a></td>
        <td width="20%" align="center"><a href= "https://github.com/sunnyineverywhere">이선의</a></td>
    </tr>
    <tr width="100%">
        <td width="20%" align="center"><img src = "https://github.com/yhjune.png"></td>
        <td width="20%" align="center"><img src = "https://github.com/sunnyineverywhere.png"/></td>
    </tr>
    <tr width="100%">
        <td width="20%" align="center">client, server</td>
        <td width="20%" align="center">server, cloud infra</td>
   </tr>
</table>

## 5. Contribute
### To-do
- [클라이언트 동적 라우팅](https://github.com/KUBER-LOUDY/kuber-loudy-front/issues/10)
- 클라이언트-서버 간 연결
- 쿠버네티스 튜토리얼 페이지 퍼블리싱
- 서버 간 카프카 메세지 연결

### Complete
- [profile 이용 config 설정](https://github.com/KUBER-LOUDY/aws-sdk-boto)
- [python sdk 이용 ec2 자동 생성](https://github.com/KUBER-LOUDY/aws-sdk-boto)
- [클라이언트 퍼블리싱 및 로그인 기능 연결](https://github.com/KUBER-LOUDY/kuber-loudy-front)
- [회원 데이터 저장 및 조회](https://github.com/KUBER-LOUDY/kuber-loudy-spring-boot)

## 6. License
이 코드는 [MIT License](https://github.com/KUBER-LOUDY/.github/blob/main/LICENSE) 하에 사용될 수 있습니다.
