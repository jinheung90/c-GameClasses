```
예전에 directx11을 공부하면서 제 나름대로 게임 엔진 비슷한 것을 만들어 보고 싶은 
마음에 만들어 봤던 코드 입니다 

솔직히 말하면 게임 엔진의 심화 내용은 까먹었고 예전에 6년전에 코드관리(github)같은것도 안 써본 때라서 없는 코드도 있고 미완성의 코드지만  
다만 제가 컴포넌트 구조를 직접 구현혔었고 이 과정에서 템플릿, 트리 구조 등등을 공부하면서 
추후에 java를 빨리 익히는데 도움이 많이 되어서 올리게 됬습니다 


```
```
사용했었던 라이브러리 및 언어

drectx11
winapi
c++ 11

```

```
주로 볼만한 클래스들 
cObject, cMainLoop, cTransform, cMonobehavior, cGameObject, cGameObjectHandle ...

cObject : 모든 클래스들의 상위클래스 (싱글톤 manager 제외)
cGameObjectHandle : cObject 관리 클래스 중간에 객체를 생성 시키거나 삭제를 할 수 있습니다 
cTransform : 좌표값과 변환 행렬을 누적시키는 메소드 등을 가지고 있는 클래스 입니다 
cGameObject : 하나의 게임 오브젝트를 지칭하는 말입니다 
cMonoBehavior : cGameObject에 로직을 붙이는 코드입니다 cCamera 등등은 이 컴포넌트를 상속받아서 씁니다 

```