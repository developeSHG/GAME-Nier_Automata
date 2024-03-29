# GAME-Nier_Automata

<img width="100%" src="https://user-images.githubusercontent.com/79896868/254760255-aa969b99-0e1c-49f6-8c32-691ee39613cb.png"/>
<h3>[DirectX 3D - Team Project] 니어오토마타</h3>

<b>동영상(Client)</b> : https://www.youtube.com/watch?v=51SftHxQRdQ 
<br/><b>동영상(Tool)</b> : https://www.youtube.com/watch?v=SsG11WXrBy0
<br/><b>장르</b> : 핵 앤 슬래시
<br/><b>날짜</b> : 2020.01.01 ~ 2020.03.01
<br/><b>인원</b> : 3명 (담당 파트 : Animation Tool, 플레이어, 몬스터, 카메라, 충돌)
<br/><b>개발 환경</b> : Visual Studio 2015 (x64)
<br/><b>개발 언어 및 도구</b> : C++, MFC, DirectX9, HLSL
<br/><b>Blog</b> : https://song-ift.tistory.com/47

<hr size="5">

* <b>디자이너가 만든 메쉬의 로컬 움직임을 그대로 재현한 Animation</b>
  - 트랙의 교체를 선형 보간을 통해 자연스럽게 표현
  - Tool을 통해 트랙의 데이터를 Test, 클라이언트로 Parsing

* <b>플레이어, 타겟의 방향과 거리를 계산해서 패턴을 결정하는 몬스터 AI</b>
  - FSM과 State Pattern을 이용해 클래스 설계 및 Animation Track 설정

* <b>Lerp(선형 보간)를 사용한 부드러운 Player Camera 이동</b>

* <b>충돌 (특정 뼈에 구체를 달아 충돌하며, 콜리전 매니저에서 중복 연산을 제어)</b>

* <b>이펙트</b>
  - 이펙트를 생성하는 Emitter와 동작을 담당하는 Module로 나누어 구현
  - 여러 Emitter들이 하나의 Particle System으로 구성
  - Catmull-Rom Spline을 사용해 부드러운 곡선의 Sword Trail 구현
