## 프레임워크 ##

+ 프론트엔드 프레임워크
  
  #### 1. Angular ####
    > 구글에서 지원하며, 양방향바인딩, 정적타입의 스크립트로 코드의 예측가능성 및 유지보수가 용이하다. 비동기 통신방식으로 SPA(Single Page Application)에서 사용한다.
  #### 2. React ####
    > 페이스북에서 지원하며, Virtual DOM을 사용하는데 이는 가상 DOM에서 처리하여, 실제 DOM에서의 리플로우, 리페인트 횟수를 줄여 빠른 성능을 보여줄 수 있다. 이는 동적 UI 생성, 운용에 유리하다.
  #### 3. Vue ####
    > Evan You 개인이 운용하며, React의 Virtual DOM과 Angular의 양방향바인딩의 장점을 모두 가져왔다.

----------------------------------------------
> 위 프레임워크들은 SPA로 되어있기 때문에, 초기 페이지(index.html) 만 전달하여 SEO(Search Engine Optimization)이 어렵다. 때문에 SSR(Server Side Rendering)이 해결책으로 나왔는데, 컨텐츠를 서버에서 렌더링하여 완성된 페이지 형태로 클라이언트에게 전달하는 방식이다. 하지만 단점으로는 성능적으로는 불필요한 탬플릿도 중복으로 로딩해야하기 때문에 느려지고, 서버렌더링에 따른 부하가 올수도 있다. 또한 모바일 앱 개발시 추가적인 백엔드 작업이 필요하다.
> > + Anguler -> Anguler Univasal
> > + React -> Next.js
> > + Vue -> Nuxt.js

---------------------------------------------
+ SSR(Server Side Rendering)

    1. 장점
        > + 검색엔진최적화(SEO)
    2. 단점
        > + 페이지 이동 시 화면 깜빡임(UX)
        > + 불필요한 탬플릿 중복 로딩(성능)
        > + 서버 렌더링에 따른 부하(성능)
        > + 모바일 앱 개발시 추가적인 백엔드 작업(생산성)
+ CSR(Client Side Rendering)
    1. 장점
        > + 첫 로딩만 기다리면 좋은 경험(UX)제공
        > + 연속된 렌더링으로 인한 과부하줄임(성능)
    2. 단점
        > + 초기 렌더링 속도가 느림(성능)
        > + SEO 최적화에 문제(성능)

