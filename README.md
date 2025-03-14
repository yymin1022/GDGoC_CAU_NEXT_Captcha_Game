## GDG on Campus CAU [NEXT: CAU]

빠른 시간 내에 ReCAPTCHA를 해제하고, 한국인만 읽을 수 있는 문장을 해석해 순위를 매기는 게임 액티비티입니다.

![image](https://github.com/yymin1022/GDGoC_CAU_NEXT_Captcha_Game/assets/12806229/5ff45af7-8646-45a1-bfaf-7dd1d7820593)

### Tech Stacks
- React.JS
- Styled Components
- [Google ReCAPTCHA API](https://developers.google.com/recaptcha/intro)

### How to Run
[Docker Pull]
1. 다음 [Dockerhub Repository](https://hub.docker.com/repository/docker/yymin1022/gdgoc-cau-captcha-game/general)를 참고하여 컨테이너 이미지를 Pull 합니다.
2. [Google ReCAPTCHA API]() 콘솔에서 웹앱을 등록하고, Key를 발급받습니다.
3. Pull 된 이미지를 기반으로 내부 80번 포트를 외부로 개설하도록 설정합니다.
4. 발급받은 Key를 `REACT_APP_GRECAPTCHA_KEY`라는 이름의 컨테이너 환경변수로 지정해주고 컨테이너를 구동합니다.

[Self Build]
1. 본 [Repository](https://github.com/yymin1022/GDGoC_CAU_NEXT_Captcha_Game)를 Clone 합니다.
2. [Google ReCAPTCHA API](https://developers.google.com/recaptcha/intro) 콘솔에서 웹앱을 등록하고, Key를 발급받습니다.
3. `.env` 파일을 생성하고, 발급받은 Key를 `REACT_APP_GRECAPTCHA_KEY` 환경변수로 지정해줍니다.
4. 프로젝트 경로로 이동해 `npm install`과 `npm start`를 수행하면 [로컬호스트 서버](http://localhost:3000)로 프로젝트가 구동됩니다.
