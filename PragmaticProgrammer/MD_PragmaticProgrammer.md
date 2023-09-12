# PragmaticProgrammer

<!-- PragmaticProgrammer 책 내용 요약 -->

[나만의 요약]--------------------------------------------------------------------------------------------------------

    - 결합도 낮춰라
    - 모듈화 해라
    - 캡슐화
    - DRY 반복하지마라
    - 직교성이 중요하다

서문--------------------------------------------------------------------------------------------------------------

    - 이 책은 더 나은 프로그래머가 되도록 돕는 책
    - 프로그래밍은 Craft 다. 프로그래밍이란 컴퓨터에게 여러분이 시키고 싶은 일을 하게끔 만드는 (또는 여러분의 고객인 사용자가 시키고 싶은 일을 하게 만드는) 것이다.
    - 도구, 언어, 운영체제든 최고의 해결방안은 없다. 오직 특정한 환경 조건의 집합마다 각 집합에 가장 적절한 시스템들이 있을 뿐
    - 실용주의란 어떤 특정 기술에 매이면 안 되며, 개별 상황마다 그 상황에서 좋은 해결방안을 고를 수 있도록 충분한 배경지식과 경험을 가져야 한다.
    - 배경지식은 컴퓨터 과학의 기본 원리들을 이해하는 것에서 나오고, 경험은 다양한 범위의 실제 프로젝트들을 수행해보는 것에서 나온다.
    - 이론과 실천의 결합이 여러분을 강하게 만든다.
    - 실용주의 프로그래머는 일을 완수한다. 그것도 아주 잘.
    - 실용주의 프로그래머는 비슷한 특징이 있다. (1) 얼리어덥터 성향 (2) 캐묻기 좋아함 (3) 비판적인 사고 (4) 현실적 (5) 다방면 기술에 익숙

 [Tip 1] 자신의 기술 (Craft)에 관심과 애정을 가져라.
 [Tip 2] 자신의 일에 대해 생각하면서 일하라!

- 우리가 단지 돌을 자를지라도 언제나 대성당을 마음속에 그려야 한다. (채석장 일꾼의 신조)
- 카이젠(Kaizen) = 지속적으로 조금씩 자주 개량하는 것을 뜻하는 일본어

1. 실용주의 철학------------------------------------------------------------------------------------------------------

[1. 고양이가 내 소스코드를 삼켰어요.]

- 실용주의 프로그래머는 무엇이 다른가? 문제 넘어를 생각하며, 문제를 더 큰 맥락에 놓으려 노력하고 더 큰 그림을 보려 한다.
- 또 다른 성공의 열쇠는 자신이 하는 모든 일에 책임을 진다는 점.
- 우리는 자신의 능력에 대해 자부심을 가질 수 있지만 실수나 무지 같은 단점에 대해서도 정직해져야 한다.

 [Tip 3] 어설픈 변명을 만들지 말고 대안을 제시하라.

- 부탁하는 것을 어려워하지 말고, 도움이 필요하다는 사실을 인정하라.

[2. 소프트웨어 엔트로피]

 [Tip 4] 깨진 창문을 내버려두지 말라.

[3. 돌멩이 수프와 삶은 개구리]

- 허락을 얻는 것보다 용서를 구하는 것이 더 쉽다.
- 무엇이 가능한지 물어보고 판단하느니 차라리 일단 저지르고 예외가 발생하면 해당 예외를 처리하게 하는 방식

 [Tip 5] 변화의 촉매가 되라.
 [Tip 6] 큰 크림을 기억하라.

[4. 적당히 괜찮은 소프트웨어]

- 어느 정도면 적당히 괜찮은지를 결정하는 과정에 사용자가 참가할 기회를 가져야 한다.
- 시스템의 범위와 품질은 요구사항으로 명기되어 있어야 한다.

 [Tip 7] 품질을 요구사항으로 만들어라.

- 사용자들에게 뭔가 직접 만져볼 수 있는 것을 일찍 준다면 피드백을 통해 더 나은 솔루션에 도달 할 수 있을 것임.
- 완벽하지 않을 수 있다. 걱정마라. 완벽해지기란 불가능하다.

[5. 지식 포트폴리오]

- 지식에 대한 투자가 언제나 최고의 이윤을 낸다. - 벤자민 프랭클린
- 지식 포트폴리오 관리는 금융 포트폴리오와 유사하다.
 [금융 포트폴리오]
  (1) 진지한 투자자들은 주기적으로 투자하는 습관이 있다. >> 소량일지라도 습관이 중요
  (2) 장기간 성공의 열쇠는 다각화다. >> 많은 기술을 익혀라.
  (3) 똑똑한 투자자들은 자신의 포트폴리오를 보수적인 투자, 위험성이 큰 투자, 보상이 높은 투자 사이에서 균형을 잘 맞춘다. >> 기술 달걀을 한 바구니에 담지마라.
  (4) 최대 수직을 위해 투자자들은 싸게 사서 비싸게 팔려고 한다. >> 새롭게 떠오르는 기술이 인기 끌기전에 미리 학습하는 것은 저평가된 주식 찾아내는 것만큼 중요
  (5) 포트폴리오는 주기적으로 재검토하고 재조정해야 한다. >> 컴퓨터 산업은 동적이다.
  
 [Tip 8] 지식 포트폴리오에 주기적으로 투자하라.

 [지식 자산을 얻는 최선의 길]
  (1) 매년 새로운 언어를 최소 하나는 배워라. >> 다른 언어는 동일한 문제를 다르게 푼다.
  (2) 기술 서적을 분기마다 한 권씩 읽어라. >> 습관이 들면 한 달에 한권씩 읽어라.
  (3) 비 기술 서적도 읽어라.(심리학, 문화인류학, 건축학, 경영학이 큰 도움됨) >> 컴퓨터를 사용하는 것은 사람이라는점을 기억해라.
  (4) 수업을 들어라. >> 근처 대학이나 시사회에서 열리는 흥미로운 강좌를 찾아보라.
  (5) 지역 사용자 모임에 참여하라. >> 가서 가만히 듣고만 오지 말고, 적극 참여하라. 고립은 경력에 치명적일 수 있다. 회사 밖에 사람들이 어떤 일을 하는지 봐라.
  (6) 다른 환경에서 실험해보라. >> 윈도우에서만 일했다면 유닉스를 갖고 놀아봐라.
  (7) 요즘 흐름을 놓치지 마라 >> 업계의 잡지와 기타 저널을 구독하라.
  (8) 인터넷을 이용해라.
  
 [Tip 9] 읽고 듣는 것을 비판적으로 분석하라.

[6. 소통하라]

- 나는 무시당하느니 차라리 샅샅이 훑어보는 시선이 낫다고 봐요. - 메이 웨스트

 [유용한 아이디어 목록]
  (1) 말하고 싶은 게 무언지 알아라. >> 무엇을 말할지 미리 계획하라. 개요를 작성하라. 그리고 자문하라. "이게 내가 말하고자 하는 것을 잘 전달하는가?" 그렇게 될 때까지 다듬어라.
  (2) 청중을 알아라. >> WISDOM >> What(무엇에), Interest(관심), sophisticated(소양), detail(구체적), own(소유), motive(동기유발)
  
- 말하는 내용만 아니라 말하는 시간도 적절하게 하라. >> 타이밍을 봐라.
- 스타일(디자인)에 신경을 써라.

 [Tip 10] 무엇을 말하는가와 어떻게 말하는가 모두 중요

2. 실용주의 접근법 ------------------------------------------------------------------------------------------------------

[7. 중복의 해악]

- 프로그래머들은 늘 유지보수 모드에 있다.
- 모든 지식은 시스템 내에서 단일하고, 애매하지 않고, 정말로 믿을만한 표현 양식을 가져야 한다.
- 신뢰성 높게 개발하고, 이해하고 유지보수하기 쉽게 만드는 유일한 길은 DRY 원칙을 지키는 것. >> Don''t Repeat Yourself

 [Tip 11] 반복하지 마라

- 돌아가는 길이 지름길이다.

 [Tip 12] 재사용하기 쉽게 만들어라.

[8. 직교성] Orthogonality

- 하나가 바뀌어도 나머지에 어떤 영향도 주지 않으면 서로 직교한다고 함.
- 헬리콥터 조종은 비직교적임 (모든 조종이 나머지 움직임에 영향을 줌)
- 직교성의 장점 >> 어느 하나를 바꿀때 나머지를 걱정안해도 됨.
  (1) 생산성 향상 >> 변화가 국소화 되서 개발 시간과 테스트 시간이 줄어든다. 재사용하기 쉽다.
  (2) 리스크 감소 >> 감염된 코드 격리 등 문제시 해당 부분만 문제됨.

 [Tip 13] 관련 없는 것들 간에 서로 영향이 없도록 하라.

- 전화번호를 키로 잡았는데 지역번호가 재할당된다면? 자신의 힘으로 제어할 수 없는 속성에 의존하지마라.
- 단위 테스트를 만든다는 것 자체가 직교성을 테스트해 볼 수 있는 흥미로운 작업임. >> 단위 테스트 하기 위해서 필요한게 뭔지 알 수 있기때문.

[9. 가역성]

- 당신이 가진 생각이 딱 하나밖에 없다면, 그것만큼 위험한 것은 없다. - 에밀 사르티에

 [Tip 14] 최종 결정이란 없다.

[10. 예광탄]

- 사용자들이 이전에 써본 적이 없기 때문에 요구사항이 막연할지도 모른다.
- 실용주의 프로그래머는 예광탄을 선호한다.

 [Tip 15] 목표물을 찾기 위해 예광탄을 써라.

- 프로토타입은 나중에 버릴 코드지만 예광탄은 기능은 별로 없지만 완결된 코드이며, 최종 시스템 골격의 일부
- 프로토타입은 예광탄이 발사되기 전에 먼저 일어나는 정찰과 정보 수집정도로 생각.

[11. 프로토타입과 포스트잇]

- 프로토타입의 대상 : 위험을 수반하는 모든 것.
- 프로토타입의 가치는 생성된 코드가 아니라 이를 통해 배우게 되는 교훈임.

 [Tip 16] 프로토타입을 통해 학습하라.

[12. 도메인 언어]

 [Tip 17] 문제 도메인에 가깝게 프로그래밍하라. ??(이해못함)

[13. 추정]

 [Tip 18] 추정을 통해 놀람을 피하라.

3. 기본적인 도구 ------------------------------------------------------------------------------------------------------

- 일을 하는 데에 더 나은 방법이 없는가 늘 주변을 살펴라.

[14. 일반 텍스트의 힘]

 [Tip 20] 지식을 일반 텍스트로 저장하라.

- 일반 텍스트는 단순, 호환성 등 장점이 많다.

[15. 조개 놀이] Shell Games

 [Tip 21] 명령어 셸의 힘을 사용하라.

[16. 파워 에디팅]

 [Tip 22] 하나의 에디터를 잘 사용하라.

[17. 소스코드 관리]

- 진보라는 것은 변화와는 거리가 멀고 오히려 기억에 의존한다. 과거를 기억하지 못하는 사람은 과거를 반복할 운명이다. - 조지 산티야나, 이성의 삶
 [Tip 23] 언제나 소스코드 관리 시스템을 사용하라.

[18. 디버깅]

 [Tip 24] 비난 대신 문제를 해결하라.
 [Tip 25] 디버깅을 할 때 당황하지 마라.

- 항상 문제의 근본적인 원인을 발견하려고 노력하고, 그 문제의 특정한 증상만 고치려고 하지 말라.
- 고무오리. 누구가에게 그걸 설명하다보면 문제에 대한 새로운 통찰을 얻을 수 있음

 [Tip 26] 'select' 는 망가지지 않았다. (시스템 보다는 우선 내가 잘못했다고 생각해라.)
 [Tip 27] 가정하지 마라. 증명하라. (무조건 맞다고 생각해도 대충 지나가지말고 증명해라.)

[19. 텍스트 처리]

 [Tip 28] 텍스트 처리 언어(python, Perl 등)를 하나 익혀라.

[20. 코드 생성기]

 [Tip 29] 코드를 작성하는 코드를 작성하라. (? IDE가 해주는듯?)

4. 실용주의 편집증 ------------------------------------------------------------------------------------------------------

 [Tip 30] 완벽한 소프트웨어는 만들 수 없다.

[21. 계약에 의한 설계]

 [Tip 31] 계약에 따른 설계를 하라.

[22. 죽은 프로그램은 거짓말을 하지 않는다]

 [Tip 32] 일찍 작동을 멈추게 하라. (불가능한 뭔가가 발생하였다면..)

[23. 단정적 프로그래밍]

 [Tip 33] 단정문(조건)을 사용해서 불가능한 상황(이런일은 절대 일어날 수 없어)을 예방하라.

[24. 언제 예외를 사용할까]

 [Tip 34] 예외는 예외적인 문제에 사용하라.

[25. 리소스 사용의 균형]

 [Tip 35] 시작한 것은 끝내라.

5. 구부러지거나 부러지거나 ------------------------------------------------------------------------------------------------------

- 유연함을 유지하는 한 가지 좋은 방법은 가능한 적은 양의 코드를 작성하는 것.

[26. 결합도 줄이기와 디미터 법칙]

- 직교성과 계약에 의한 설계에서 *shy 코드를 작성하는 것이 이롭다고 했다.
- 여기서 shy 코드란, 자신을 남에게 속속들이 드러내지 말고, 너무 많은 사람과 상호작용하지 말라는 두 가지 의미를 모두 내포한다.
- 코드를 모듈로 구성하고 이들 간의 상호작용을 제한하라. 그러면 한 모듈이 변경되거나 교체된다 하더라도 다른 모듈은 변경없이 작동 가능할 것.
- 의존도를 최소화하기 위해 디미터 법칙을 사용하여 메서드, 함수를 설계한다.

 [Tip 36] 모듈간의 결합도를 최소화하라. (디미터 법칙을 이용 ?)

- DB 스키마 설계시 반정규화로 성능을 개선하는 것처럼 모듈 결합도를 높여서 중요한 성능향상을 얻을 수 있지만 이게 아니라면 결합도 높여놓으면 미래는 없다고 봐야함.

[27. 메타프로그래밍]

 [Tip 37] 통합하지 말고 설정하라.

- 메타데이터? 데이터에 관한 데이터 (DB스키마 같은것) (넓은 의미로는 애플리케이션을 기술하는 모든 데이터)

 [Tip 38] 코드에는 추상화를, 메타데이터에는 세부 내용을 (?)

- 이렇게 하면 설계의 결합도를 줄여 좀 더 유연하고 적응성 있는 프로그램이 된다.
- 세부사항을 코드 밖으로 몰아냄으로써 보다 강하고 추상적인 디자인을 만들 수 있다.

- 프로그램이 실행 중에도 설정 정보를 리로딩할 수 있도록 만들어라.
- 환경에 적응하지 못하는 종(도도)은 멸종한다.

[28. 시간적 결합]

 [Tip 39] 작업흐름 분석을 통해 동시성을 개선하라.
 [Tip 40] 서비스를 사용해서 설계하라.
 [Tip 41] 언제나 동시성을 고려해 설계하라.

- 동시성을 허용하여 설계한다면, 확장가능성이나 성능에 대한 요구사항이 있을때 더 수비게 처리 가능하며 항상 깔끔한 설계의 이점을 가진다.

[29. 단지 뷰일 뿐이야]

- 이벤트를 이용하면 어떤 객체의 상태 변화를 이에 관심을 가질 다른 객체들에게 알릴 수 있다.
 [모델-뷰-컨트롤러] 모델을 표시하는 뷰 그리고 뷰를 관리하는 컨트롤러에서 모델을 분리해 내는 것. 이것이 MVC 의 핵심 개념

 [Tip 42] 모델에서 뷰를 분리하라.

[30. 칠판]

 [Tip 43] 칠판을 사용해 작업흐름을 조율하라.

6. 코딩하는 동안 해야 할 일들 ------------------------------------------------------------------------------------------------------

- 적극적으로 자기 코드에 대해 생각하지 않는 프로그래머는 우연에 맡기는 프로그래밍을 하는 것.  
- 운전을 안전하게 잘하는 사람들은 언제나 자기 상황을 검토하고, 잠재적인 문제들을 점검하며, 예상하지 못한 일이 생겼을 때에도 잘 대처한다.
- 코딩도 대부분 반복적인 일이지만 마음을 늘 깨어있도록 유지하면 재앙을 막을 수 있다.

[31. 우연에 맡기는 프로그래밍]

- 우리는 우연에 맡기는 프로그래밍 대신 의도적으로 프로그래밍 해야한다.
- 코드가 왜 안돌아가는지 모르는 이유는 왜 돌아가는지 모르기 때문이다.

 [Tip 44] 우연에 맡기는 프로그래밍을 하지 말라.

 [의도적으로 프로그래밍하기]

- 언제나 자기가 지금 무엇을 하고 있는지 알아야 한다.
- 맹목적으로 코딩하지 말라.
- 계획을 세우고 계획을 바탕으로 진행하라.
- 신뢰할 수 있는 것에만 기대라. 일단 가장 최악의 상황을 가정하라.
- 여러분의 가정을 문서로 남겨라.
- 노력을 기울일 대상의 우선순위를 정하라.
- 과거의 노예가 되지 말라.

[32. 알고리즘의 속도]

 [상식적인 추정]

- 간단한 반복문, 만약 간단한 반복문 하나가 1부터 n까지 돌아간다면, 이 알고리즘이 O(n) 일 가능성이 높다. 즉 수행시간은 n과 비례해서 증가.
- 겹친 반복문,
- 반씩 잘라 나가기
- 나눠서 정복하기
- 조합적
  
 [Tip 45] 여러분 알고리즘의 차수를 추정하라.
 [Tip 46] 여러분의 추정을 테스트하라.

- 어떤 알고리즘을 개선하기 전에 정말로 병목인지 확실히 해두는게 좋은 생각이다.

[33. 리팩터링]

- 소프트웨어 개발은 정원일에 가깝다.
- 코드 다시 작성, 다시 작업, 다시 설계 등을 리팩터링이라고 한다.

 [언제 리팩터링?]

- 언제나 바로 지금이 최적기.
- 중복 : DRY 원칙의 위반
- 직교성이 좋지 않은 설계
- 유효기간이 끝난 지식
- 성능 개선
- 현실을 피하지 말자.
- 리팩터링은 종양제거와 같다. 빨리 안하면 더 큰 비용을 지불해야한다.
  
 [Tip 47] 일찍 리팩터링하고, 자주 리팩터링하라.

 [리팩터링 조언]
  (1) 리팩터링과 새로운 기능 추가를 동시에 하지 말라.
  (2) 자주 테스트를 돌려보면서 해라.
  (3) 단계를 나누어서 신중하게 작업한다.
  
- 지금 고통스럽더라도, 앞으로 더욱 고통스러워질 것 같으면 지금 고치는 편이 낫다.
- 깨진 창문을 그대로 두지 말라.

[34. 테스트하기 쉬운 코드]

 [Tip 48] 테스트를 염두에 두고 설계하라.
 [Tip 49] 소프트웨어를 테스트하라. 그렇지 않으면 사용자가 테스트하게 될 것이다.

[35. 사악한 마법사]

- 코드를 정말로 이해하지 못하는 한 자기 자신을 속이는 것

 [Tip 50] 자신이 이해하지 못하는, 마법사가 만들어 준 코드는 사용하지 말라.
  
7. 프로젝트 전에 ------------------------------------------------------------------------------------------------------

[36. 요구사항의 구렁텅이]

- 완성이라는 것은 더 이상 더할 것이 없을 때가 아니라, 더 이상 빼낼 것이 없을 때 얻게 되는 것. - 생텍쥐페리

 [Tip 51] 요구사항을 수집하지 말고 채굴하라.
  
 *인사부서만 열람할 수 있다로 만들지말고 권한이 있는 부서만 열람할 수 있다로 만들어라.

- 사용자들이 어떤 작업을 현재 어떻게 하느냐는 것을 알아내는 것보다, 왜 그걸 하는지 그 내재적 이유를 알아내는 것이 더 중요하다.
- 개발을 통해서 요구사항을 충족시키는게 아니라 실질적 비지니스 문제를 해결하는 것이다.

 [Tip 52] 사용자처럼 생각하기 위해 사용자와 함께 일하라.
 [Tip 53] 구체적인 것보다 추상적인 것이 더 오래간다.
 [Tip 54] 프로젝트 용어사전을 사용하라.

[37. 불가능한 퍼즐 풀기]

 [Tip 55] 생각의 틀을 벗어나지 말고, 틀을 찾아라.

 [불가능한 문제가 있다면]

- 더 쉬운 방법이 존재하는가?
- 진짜 문제를 풀려고 노력하고 있나. 그렇지 않다면 중요하지 않은 기술적 문제에 정신이 팔려 있는 것인가?
- 왜 이것이 문제인가?
- 문제를 이렇게 풀기 어렵게 만드는 것이 무엇인가?
- 반드시 이 방법으로 해야 하는가?
- 반드시 해야 하는 일이긴 한가?
  
[38. 준비가 되어야만]

 [Tip 56] 준비가 되었을 때 시작하라.

[39. 명세의 함정]

 [Tip 57] 어떤 일들은 설명하기보다 실제로 하는 것이 쉽다.

- 프로토타이핑을 해보거나, 예광탄 개발을 고려해봐라

[40. 동그라미와 화살표]

 [Tip 58] 형식적 방법의 노예가 되지 마라.
 [Tip 59] 비싼 도구가 더 좋은 설계를 낳지는 않는다.

8. 실용주의 프로젝트 ------------------------------------------------------------------------------------------------------

[41. 실용주의 팀]

- 깨진 창문을 없애라.
- 품질은 팀원 '전체'가 개인적으로 기여할 때만 보장된다.
- 모든 사람이 적극적으로 환경 변화를 감시해야 한다.
- 소통하라! 프로젝트명을 지어서 사용하면 좋다.
- 반복하지 마라.
- 직교성
 [Tip 60] 팀을 기능 중심으로 조직하라.
- 변화가 생기더라도 전체가 영향 받는 일이 없게 된다.

[42. 유비쿼터스 자동화]

- 생각 없이 행할 수 있는 중요한 작업의 수가 늘어남에 따라 문명은 발전한다. - 알프레드 노스 화이트헤드
 [Tip 61] 수작업 절차를 사용하지 마라. (각자 다 다르게 한다..)

[43. 가차 없는 테스트]

 [Tip 62] 일찍 테스트하고, 자주 테스트하라. 자동으로 테스트하라.
 [Tip 63] 모든 테스트가 통과하기 전엔 코딩이 다 된 게 아니다.

 [무엇을 테스트할지, 어떻게 테스트할지, 언제 테스트할지]

 [수행해야할 소프트웨어 테스트]

- 단위 테스트 : 하나의 모듈 테스트
- 통합 테스트
- 유효성 평가와 검증
- 자원 고갈, 에러, 그리고 복구
- 성능 테스트
- 사용편의성 테스트

-------------------------------------------------------------------------------------------------------------------PragmaticProgrammer.com

[Tip]  #1, pg. xxi:

Care About Your Craft
Why spend your life developing software unless you care about doing it well?

[Tip]  #2, pg. xxi:

Think! About Your Work
Turn off the autopilot and take control. Constantly critique and appraise your work.

[Tip]  #3, pg. 2:

You Have Agency
It’s your life. Grab hold of it and make it what you want.

[Tip]  #4, pg. 4:

Provide Options, Don’t Make Lame Excuses
Instead of excuses, provide options. Don’t say it can’t be done; explain what can be done.

[Tip]  #5, pg. 7:

Don’t Live with Broken Windows
Fix bad designs, wrong decisions, and poor code when you see them.

[Tip]  #6, pg. 9:

Be a Catalyst for Change
You can’t force change on people. Instead, show them how the future might be and help them participate in creating it.

[Tip]  #7, pg. 10:

Remember the Big Picture
Don’t get so engrossed in the details that you forget to check what’s happening around you.

[Tip]  #8, pg. 12:

Make Quality a Requirements Issue
Involve your users in determining the project’s real quality requirements.

[Tip]  #9, pg. 15:

Invest Regularly in Your Knowledge Portfolio
Make learning a habit.

[Tip]  #10, pg. 17:

Critically Analyze What You Read and Hear
Don’t be swayed by vendors, media hype, or dogma. Analyze information in terms of you and your project.

[Tip]  #11, pg. 20:

English is Just Another Programming Language
Treat English as Just Another Programming Language. Write documents as you would write code: honor the DRY principle, ETC, automation, and so on.

[Tip]  #12, pg. 22:

It’s Both What You Say and the Way You Say It
There’s no point in having great ideas if you don’t communicate them effectively.

[Tip]  #13, pg. 23:

Build Documentation In, Don’t Bolt It On
Documentation created separately from code is less likely to be correct and up to date.

[Tip]  #14, pg. 28:

Good Design Is Easier to Change Than Bad Design
A thing is well designed if it adapts to the people who use it. For code, that means it must adapt by changing.

[Tip]  #15, pg. 31:

DRY—Don''t Repeat Yourself
Every piece of knowledge must have a single, unambiguous, authoritative representation within a system.

[Tip]  #16, pg. 38:

Make It Easy to Reuse
If it’s easy to reuse, people will. Create an environment that supports reuse.

[Tip]  #17, pg. 40:

Eliminate Effects Between Unrelated Things
Design components that are self-contained, independent, and have a single, well-defined purpose.

[Tip]  #18, pg. 48:

There Are No Final Decisions
No decision is cast in stone. Instead, consider each as being written in the sand at the beach, and plan for change.

[Tip]  #19, pg. 49:

Forgo Following Fads
Neal Ford says, “Yesterday’s Best Practice Becomes Tomorrow’s An[Tip] attern.” Choose architectures based on fundamentals, not fashion.

[Tip]  #20, pg. 51:

Use Tracer Bullets to Find the Target
Tracer bullets let you home in on your target by trying things and seeing how close they land.

[Tip]  #21, pg. 57:

Prototype to Learn

Prototyping is a learning experience. Its value lies not in the code you produce, but in the lessons you learn.

[Tip]  #22, pg. 60:

Program Close to the Problem Domain

Design and code in the language of the problem domain.

[Tip]  #23, pg. 66:

Estimate to Avoid Surprises

Estimate before you start. You’ll spot potential problems up front.

[Tip]  #24, pg. 70:

Iterate the Schedule with the Code

Use experience you gain as you implement to refine the project time scales.

[Tip]  #25, pg. 75:

Keep Knowledge in Plain Text

Plain text won’t become obsolete. It helps leverage your work and simplifies debugging and testing.

[Tip]  #26, pg. 79:

Use the Power of Command Shells

Use the shell when graphical user interfaces don’t cut it.

[Tip]  #27, pg. 81:

Achieve Editor Fluency

An editor is your most important tool. Know how to make it do what you need, quickly and accurately.

[Tip]  #28, pg. 85:

Always Use Version Control

Version control is a time machine for your work; you can go back.

[Tip]  #29, pg. 89:

Fix the Problem, Not the Blame

It doesn’t really matter whether the bug is your fault or someone else’s—it is still your problem, and it still needs to be fixed.

[Tip]  #30, pg. 89:

Don’t Panic

This is true for galactic hitchhikers and for developers.

[Tip]  #31, pg. 91:

Failing Test Before Fixing Code

Create a focussed test that reveals the bug before you try fixing it.

[Tip]  #32, pg. 92:

Read the Damn Error Message

Most exceptions tell both what failed and where it failed. If you’re lucky you might even get parameter values.

[Tip]  #33, pg. 95:

“select” Isn''t Broken

It is rare to find a bug in the OS or the compiler, or even a third-party product or library. The bug is most likely in the application.

[Tip]  #34, pg. 96:

Don’t Assume It—Prove It

Prove your assumptions in the actual environment—with real data and boundary conditions.

[Tip]  #35, pg. 98:

Learn a Text Manipulation Language

You spend a large part of each day working with text. Why not have the computer do some of it for you?

[Tip]  #36, pg. 102:

You Can’t Write Perfect Software

Software can’t be perfect. Protect your code and users from the inevitable errors.

[Tip]  #37, pg. 107:

Design with Contracts

Use contracts to document and verify that code does no more and no less than it claims to do.

[Tip]  #38, pg. 113:

Crash Early

A dead program normally does a lot less damage than a crippled one.

[Tip]  #39, pg. 115:

Use Assertions to Prevent the Impossible

If it can’t happen, use assertions to ensure that it won’t. Assertions validate your assumptions. Use them to protect your code from an uncertain world.

[Tip]  #40, pg. 118:

Finish What You Start

Where possible, the function or object that allocates a resource should be responsible for deallocating it.

[Tip]  #41, pg. 121:

Act Locally

Keep the scope of mutable variables and open resources short and easily visible.

[Tip]  #42, pg. 126:

Take Small Steps—Always

Small steps always; check the feedback; and adjust before proceeding.

[Tip]  #43, pg. 127:

Avoid Fortune-Telling

Only look ahead as far as you can see.

[Tip]  #44, pg. 131:

Decoupled Code Is Easier to Change

Coupling ties things together, so that it’s harder to change just one thing.

[Tip]  #45, pg. 132:

Tell, Don’t Ask

Don’t get values from an object, transform them, and then stick them back. Make the object do the work.

[Tip]  #46, pg. 134:

Don’t Chain Method Calls

Try not to have more than one dot when you access something.

[Tip]  #47, pg. 136:

Avoid Global Data

It’s like adding an extra parameter to every method.

[Tip]  #48, pg. 136:

If It’s Important Enough To Be Global, Wrap It in an API

…but only if you really, really want it to be global.

[Tip]  #49, pg. 149:

Programming Is About Code, But Programs Are About Data

All programs transform data, converting an input into an output. Start designing using transformations.

[Tip]  #50, pg. 153:

Don’t Hoard State; Pass It Around

Don’t hang on to data within a function or module. Take one down and pass it around.

[Tip]  #51, pg. 161:

Don''t Pay Inheritance Tax

Consider alternatives that better fit your needs, such as interfaces, delegation, or mixins

[Tip]  #52, pg. 162:

Prefer Interfaces to Express Polymorphism

Interfaces make polymorphism explicit without the coupling introduced by inheritance.

[Tip]  #53, pg. 163:

Delegate to Services: Has-A Trumps Is-A

Don’t inherit from services: contain them.

[Tip]  #54, pg. 165:

Use Mixins to Share Functionality

Mixins add functionality to classes without the inheritance tax. Combine with interfaces for painless polymorphism.

[Tip]  #55, pg. 166:

Parameterize Your App Using External Configuration

When code relies on values that may change after the application has gone live, keep those values external to the app. When you application will run in different environments, and potentially for different customers, keep the environment and customer specific values outside the app.

[Tip]  #56, pg. 171:

Analyze Workflow to Improve Concurrency

Exploit concurrency in your user’s workflow.

[Tip]  #57, pg. 174:

Shared State Is Incorrect State

Shared state opens a large can of worms that can often only be fixed by rebooting.

[Tip]  #58, pg. 180:

Random Failures Are Often Concurrency Issues

Variations in timing and context can expose concurrency bugs, but in inconsistent and irreproducible ways.

[Tip]  #59, pg. 182:

Use Actors For Concurrency Without Shared State

Use Actors to manage concurrent state without explicit synchronization.

[Tip]  #60, pg. 189:

Use Blackboards to Coordinate Workflow

Use blackboards to coordinate disparate facts and agents, while maintaining independence and isolation among participants.

[Tip]  #61, pg. 194:

Listen to Your Inner Lizard

When it feels like your code is pushing back, it’s really your subconscious trying to tell you something’s wrong.

[Tip]  #62, pg. 200:

Don’t Program by Coincidence

Rely only on reliable things. Beware of accidental complexity, and don’t confuse a happy coincidence with a purposeful plan.

[Tip]  #63, pg. 207:

Estimate the Order of Your Algorithms

Get a feel for how long things are likely to take before you write code.

[Tip]  #64, pg. 208:

Test Your Estimates

Mathematical analysis of algorithms doesn’t tell you everything. Try timing your code in its target environment.

[Tip]  #65, pg. 212:

Refactor Early, Refactor Often

Just as you might weed and rearrange a garden, rewrite, rework, and re-architect code when it needs it. Fix the root of the problem.

[Tip]  #66, pg. 214:

Testing Is Not About Finding Bugs

A test is a perspective into your code, and gives you feedback about its design, api, and coupling.

[Tip]  #67, pg. 216:

A Test Is the First User of Your Code

Use its feedback to guide what you do.

[Tip]  #68, pg. 218:

Build End-To-End, Not Top-Down or Bottom Up

Build small pieces of end-to-end functionality, learning about the problem as you go.

[Tip]  #69, pg. 221:

Design to Test

Start thinking about testing before you write a line of code.

[Tip]  #70, pg. 223:

Test Your Software, or Your Users Will

Test ruthlessly. Don’t make your users find bugs for you.

[Tip]  #71, pg. 224:

Use Property-Based Tests to Validate Your Assumptions

Property-based tests will try things you never thought to try, and exercise your code in ways is wasn’t meant to be used.

[Tip]  #72, pg. 234:

Keep It Simple and Minimize Attack Surfaces

Complex code creates a breeding ground for bugs and opportunities for attackers to exploit.

[Tip]  #73, pg. 235:

Apply Security Patches Quickly

Attackers deploy exploits as quick as they can, you have to be quicker.

[Tip]  #74, pg. 242:

Name Well; Rename When Needed

Name to express your intent to readers, and rename as soon as that intent shifts.

[Tip]  #75, pg. 244:

No One Knows Exactly What They Want

They might know a general direction, but they won’t know the twists and turns.

[Tip]  #76, pg. 245:

Programmers Help People Understand What They Want

Software development is an act of co-creation between users and programmers.

[Tip]  #77, pg. 246:

Requirements Are Learned in a Feedback Loop

Understanding requirements requires exploration and feedback, so the consequences of decisions can be used to refine the initial ideas.

[Tip]  #78, pg. 247:

Work with a User to Think Like a User

It’s the best way to gain insight into how the system will really be used.

[Tip]  #79, pg. 248:

Policy Is Metadata

Don’t hardcode policy into a system; instead express it as metadata used by the system.

[Tip]  #80, pg. 251:

Use a Project Glossary

Create and maintain a single source of all the specific terms and vocabulary for a project.

[Tip]  #81, pg. 254:

Don’t Think Outside the Box—Find the Box

When faced with an impossible problem, identify the real constraints. Ask yourself: “Does it have to be done this way? Does it have to be done at all?”

[Tip]  #82, pg. 259:

Don''t Go into the Code Alone

Programming can be difficult and demanding. Take a friend with you.

[Tip]  #83, pg. 259:

Agile Is Not a Noun; Agile Is How You Do Things

Agile is an adjective: it’s how you do something.

[Tip]  #84, pg. 264:

Maintain Small Stable Teams

Teams should be small and stable, where everyone trusts each other and depends on each other.

[Tip]  #85, pg. 266:

Schedule It to Make It Happen

If you don’t schedule it, it’s not going to happen. Schedule reflection, experimentation, learning and skills improvement.

[Tip]  #86, pg. 268:

Organize Fully Functional Teams

Organize Around Functionality, Not Job Functions. Don’t separate UI/UX designers from coders, frontend from backend, testers from data modelers, design from deployment. Build teams so you can build code end-to-end, incrementally and iteratively.

[Tip]  #87, pg. 271:

Do What Works, Not What’s Fashionable

Don’t adopt a development method or technique just because other companies are doing it. Adopt what works for your team, in your context.

[Tip]  #88, pg. 273:

Deliver When Users Need It

Don’t wait weeks or months to deliver just because your process demands it.

[Tip]  #89, pg. 274:

Use Version Control to Drive Builds, Tests, and Releases

Use commits or pushes to trigger builds, tests, releases. Use a version control tag to deploy to production.

[Tip]  #90, pg. 275:

Test Early, Test Often, Test Automatically

Tests that run with every build are much more effective than test plans that sit on a shelf.

[Tip]  #91, pg. 275:

Coding Ain’t Done ’Til All the Tests Run

’Nuff said.

[Tip]  #92, pg. 277:

Use Saboteurs to Test Your Testing

Introduce bugs on purpose in a separate copy of the source to verify that testing will catch them.

[Tip]  #93, pg. 278:

Test State Coverage, Not Code Coverage

Identify and test significant program states. Testing just lines of code isn’t enough.

[Tip]  #94, pg. 278:

Find Bugs Once

Once a human tester finds a bug, it should be the last time a human tester finds that bug. Automatic tests should check for it from then on.

[Tip]  #95, pg. 279:

Don''t Use Manual Procedures

A computer will execute the same instructions, in the same order, time after time.

[Tip]  #96, pg. 281:

Delight Users, Don’t Just Deliver Code

Develop solutions that produce business value for your users and delight them every day.

[Tip]  #97, pg. 282:

Sign Your Work

Artisans of an earlier age were proud to sign their work. You should be, too.

[Tip]  #98, pg. 286:

First, Do No Harm

Failure is inevitable. Make sure no one will suffer because of it.

[Tip]  #99, pg. 287:

Don’t Enable Scumbags

Because you risk becoming one, too.

[Tip]  #100, pg. 287:

It’s Your Life. Share it. Celebrate it. Build it. AND HAVE FUN!

Enjoy this amazing life we have, and do great things.
