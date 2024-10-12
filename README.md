# UnrealProject_IATD(Interactive Art by TouchDesigner)
UNREAL(BP) PROJECT


![image](https://github.com/user-attachments/assets/2e5d4c78-0088-4319-a5b2-ecd5689c473a)


[교내 시행 개인 인터랙티브 아트 프로젝트, 블루프린트 기반 언리얼엔진5을 이용하여 제작]





[구현 영상]

https://youtu.be/UJId34eI3Rg





[사용툴]

Cinema4D, 언리얼엔진5, TouchDesigner






[목적]

블루프린트 기반 언리얼엔진으로 맵을 구현한 뒤, 터치디자이너 프로그램 내부에서 콘솔 컨트롤러와의 연동을 통해 Interactive Art를 구현함

인터렉티브 아트 프로젝트의 구현 및 언리얼의 통신, 각종 에셋 제작의 실력향상 목표





[컨셉]

플레이어가 이터널 홀(무한 터널)을 지나가면서 컨트롤러 조작을 통해 맵의 회전, 조명효과, 속도 증가등의 효과 부여






[맵제작 참고]

https://youtu.be/ydkiYtiwDas?si=gJSuuISDm-Cm-CyY





[제작 방법]

Cinema4D 를 이용해 맵 틀 제작
언리얼엔진(블루프린트 기반)으로 기본적인 맵 제작, 에셋 제작 





[구동원리]

-> OWL 플러그인을 이용하여 OSC 통신을 통해 언리얼엔진에서 터치디자이너로 언리얼 맵 정보 전송 

-> 언리얼에서 전송하는 신호를 터치디자이너에서 받아 음악에 맞는 맵 요소(X, Y 좌표 및 회전률, 배속 등)로 변환

-> 터치디자이너에서 컨트롤러 입력을 받아 맵의 회전, 조명효과, 배속에 관한 파라미터를 조절함

-> OSC 서버 통신을 통해 갱신된 파라미터들을 언리얼엔진으로 다시 전송함

-> 해당 파라미터를 통해 언리얼엔진에서 시스템을 구현

-> 반복
