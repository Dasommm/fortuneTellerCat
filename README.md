# 챗GPT를 사용한 운세 챗봇
- 2023.03

## 개발 목표

- 날짜와 태어난 시간을 입력하여 나만의 운세 보기

## 개발 환경

- 개발 툴
    - VSCode
- 사용 기술
    - Frontend : JavaScript, HTML, CSS
    - Backend : Node.js, JavaScript, Express, OpenAl, AWS
    - 사용한 npm 모듈 : cors, express, openai, serverless-http
    - 배포 :
        - Frontend : cloudflare
        - Backend : AWS Lambda, API Gateway

## 구현 기능

- 사용자의 생년월일과 태어난 시간을 받은 후 채팅화면 구현
    
    <img width="424" height="523" alt="1" src="https://github.com/user-attachments/assets/f5a4ac1c-3405-421c-aa4a-b3b00dd661ea" />

    
- OpenAI를 사용하여 시스템이 운세를 볼 수 있도록 프롬프트를 작성한 후 사용자가 입력한 생년월일과 태어난 시간을 기반으로 운세를 볼 수 있도록 구현
    
   <img width="532" height="413" alt="2" src="https://github.com/user-attachments/assets/0ecc1f05-5b3a-417c-bbf1-745394b912aa" />

    
    <img width="532" height="413" alt="3" src="https://github.com/user-attachments/assets/f047a8b9-3b0b-4b22-ab9f-128e78e5405f" />

    
    <img width="532" height="413" alt="4" src="https://github.com/user-attachments/assets/e6d0eb50-09be-4c24-b96c-f6de58fccda9" />

    

## 문제점

1. gpt-3.5turbo를 사용하고 있는데, 종종 응답이 너무 느린 경우가 있음. API Gateway의 응답 제한시간이 최대 29초인데 이 안에 들어오지 못하는 경우가 있어서 타임아웃 발생

---

## 버전

### V2. 
2023.11.17

- API 호출 방식 및 응답 형식이 변경되어 backend 호출 방법 및 응답 형식 수정

[I 'm using Openai api in nodeJS but throwing error](https://community.openai.com/t/i-m-using-openai-api-in-nodejs-but-throwing-error/325705)

[v3 to v4 Migration Guide · openai/openai-node · Discussion #217](https://github.com/openai/openai-node/discussions/217)
