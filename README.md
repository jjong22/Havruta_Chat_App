# Havruta_Chat_App
안녕하세요! 세마고등학교 Maker 프로젝트 팀 PathFinder 입니다.   
이 앱은 저희가 만든 챗봇을 Kommunicate SDK와 연동하여 만든 앱입니다.   
챗봇에게 질문하며 복습할 수 있게 만들어진 챗봇 앱입니다.   

![chatscreen](https://user-images.githubusercontent.com/61818473/139840147-d715b234-bcce-42f8-b13d-3b14b43d7b2e.png)

챗봇에 대한 자세한 내용을 알고 싶으시다면 다음 글을 참조해 주세요!   
https://blog.naver.com/jjong222222/222508155703   

저희가 만든 앱을 따라 만들어 볼 수 있도록 아래에 저희가 진행한 방법을 기록해 놓았습니다!   
여러분들도 챗봇을 만들어 볼 수 있는 기회가 되었으면 좋겠습니다.   

준비물 :    
Android Studio - https://developer.android.com/studio   
결제 정보가 등록된 Google Cloud 계정 - https://cloud.google.com/   
Dialogflow - https://dialogflow.cloud.google.com   
Kommunicate - https://www.kommunicate.io/   

먼저 Dialogflow를 활용하여 챗봇을 제작해야 합니다.   
<img width="960" alt="챗봇 화면" src="https://user-images.githubusercontent.com/61818473/139840829-931bce27-bf81-4b5e-b7e2-ce21c0a31230.PNG">   
(Dialogflow 화면)   

Dialogflow를 활용하여 챗봇을 만드는 과정은 생각보다 어렵지 않습니다.   
먼저 사진 위에 보이는 Intent를 추가해 사용자 응답을 받고, 챗봇이 할 대화를 입력해 주면 됩니다.   

저희가 이용한 참고 자료는 다음과 같습니다. 챗봇을 제작하는데 도움이 되었으면 좋겠습니다.   
동빈나 - https://www.youtube.com/watch?v=WLUEghtVS9k&list=PLRx0vPvlEmdCb33sBZGXzVOMY_seqnWJT   
구글 클라우드 가이드 - https://cloud.google.com/dialogflow/docs   

그 다음은 제작한 챗봇을 연동할 차례입니다.      
Dialogflow에서 제공하는 연동 기능을 사용하려 했지만, 저희는 그 방법에 어려움을 겪어 Kommunicate앱을 사용하여 연동하였습니다.      

<img width="959" alt="키 연동" src="https://user-images.githubusercontent.com/61818473/139841487-4917c878-d8e7-4959-aaf0-74acf943b6da.PNG">

먼저 구글 클라우드를 사용할 수 있는 결제 정보를 입력한 계정이 필요합니다.   
그 다음 <IAM 및 관리자> 창에 있는 "IAM"에서 제작한 챗봇, Dialogflow에 접근할 수 있는 관리자 계정을 추가합니다.   
그리고, 위 사진처럼 "서비스 계정"에서 키를 발급받습니다.   

** 키를 발급하면 .json 형태의 파일로 다운로드가 됩니다. 발급 받은 키를 분실하지 않도록 합시다! **   

자세한 내용은 다음 글을 참고해 주세요!   
https://naulsnow.tistory.com/7   

<img width="960" alt="bot integrations" src="https://user-images.githubusercontent.com/61818473/139841907-19dde3e1-771d-46d8-a20b-360568acdaaa.PNG">   
Kommunicate에 있는 <Bot Integration>에 발급한 키를 넣어 만든 챗봇을 Kommunicate 사이트에 업로드 할 수 있습니다.   
  
그 다음 저희는 Kommunicate에서 제공하는 SDK를 사용하여 앱을 제작하였습니다.   
Kommunicate SDK - https://github.com/Kommunicate-io/Kommunicate-Android-Chat-SDK   
  
또한, Kommunicate에서 제공하는 연동 기능을 사용하여 쉽게 페이스북 등 다른 사이트와 연동할 수도 있습니다.   
저희는 이 기능을 사용하여 Facebook과 연동하여, 앱 다운없이 챗봇을 사용할 수 있게 제작하기도 하였습니다.   
페이스북 페이지 https://www.facebook.com/mungtaengi11   
<img width="892" alt="연동" src="https://user-images.githubusercontent.com/61818473/139842778-a49c3250-8414-4455-958b-50af406f40fc.PNG">   
(다양한 연동 기능)   
  
저희의 연구가 챗봇을 제작해 보고 싶은 사람들에게 도움이 되었으면 좋겠습니다!!   
감사합니당   

