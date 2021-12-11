# Quest 01. HTML과 웹의 기초

## Introduction

- HTML은 HyperText Markup Language의 약자로, 웹 브라우저에 내용을 표시하기 위한 가장 기본적인 언어입니다. 이번 퀘스트를 통해 HTML에 관한 기초적인 사항들을 알아볼 예정입니다.

## Topics

- HTML의 역사
  - HTML 4.01, XHTML 1.0, XHTML 1.1
  - XHTML 2.0과 HTML5의 대립
  - HTML5와 현재
- 브라우저의 역사
  - Mosaic와 Netscape
  - Internet Explorer의 독점시대
  - Firefox와 Chrome의 등장
  - iOS Safari와 모바일 환경의 브라우저
  - Edge와 Whale 등의 최근의 Chromium 계열 브라우저
- HTML 문서의 구조
  - `<html>`, `<head>`와 `<body>` 등의 HTML 문서의 기본 구조
  - 시맨틱 엘리먼트
  - 블록 엘리먼트와 인라인 엘리먼트의 차이

## Resources

- [MDN - HTML](https://developer.mozilla.org/ko/docs/Web/HTML)
- [HTML For Beginners](https://html.com/)
- [History of the web browser](https://en.wikipedia.org/wiki/History_of_the_web_browser)
- [History of HTML](https://en.wikipedia.org/wiki/HTML)
- [StatCounter](https://gs.statcounter.com/)

## Checklist

- **HTML 표준의 역사는 어떻게 될까요?**

  HTML은 웹페이지의 컨텐츠들을 다양한 환경(브라우저)에서 열람을 해도 동일하게 볼 수 있도록 하기 위해 기존에 존재하던 SGML(Standard Generalized Markup Language)이라는 문서용 마크업 언어를 정의하기 위한 메타언어를 기반으로 웹에 알맞게 필요한 것들을 가져와 만들어졌다.

  1. 팀 버너스리에 의해 설계되어 HTTP, URI, 브라우저와 함께 1990년에 개발

  2. 1993년 HTML 1.0이 표준으로 등장, IETF(Internet Engineering Task Force) HTML Working Group에서 관리

  3. 1995년 HTML 2.0은 [RFC 1866](https://datatracker.ietf.org/doc/html/rfc1866)로서 표준화

  4. 1997년 HTML 3.2은 팀 버너스리를 중심으로 각종 기관들이 모여서 웹의 표준을 정의하는 국제 컨소시엄 W3C에 의해 [W3C Recommendation](https://www.w3.org/TR/2018/SPSD-html32-20180315/)으로 게시됨. IETF가 1996년 9월 12일 HTML Working Group을 폐쇄함에 따라 W3C가 독점적으로 개발하고 표준화한 첫 번째 버전.

  5. 1999년 HTML 4.01이 [W3C Recommendation](https://www.w3.org/TR/html401/)으로 게시됨. **CSS(Cascading Style Sheet)로 디자인적인 요소를 구분하게 되고, HTML로는 웹페이지의 전반적인 구조만을 명시하는 것을 원칙으로 하게 됨**. 이후 W3C에서는 이제 HTML은 다양화된 웹페이지를 모두 표현하기에 기술적인 한계에 부딛혔다고 판단하고, 더이상 HTML을 발전시키지 않을 것을 공표하게 된다.

  6. 2000년 XHTML 1.0이 새로운 표준으로 [W3C Recommendation](https://www.w3.org/TR/xhtml1/)으로 게시됨. XHTML은 XML과 HTML을 합성하여 더 확장된 태그를 사용할 수 있으며, 문법은 정확히 지켜지지 않는다면 표현되지 않도록 문법 검사를 엄격하게 적용하였다. 그러나 XML은 버전과 버전사이의 하위 호환성을 지원하지 않아서 이전의 태그들로 작성된 것들이 사용되지 않을 수 있다는 문제점이 있었고, 문법이 엄격하여 습득에 어려움을 느껴 표준화에 실패하게 된다.

  7. 2004년 Apple, Mozilla, Opera는 HTML을 계승하는 표준을 만들기 위해 공동으로 WHATWG(Web Hypertext Application Technology Working Group)를 발족. 2007년 W3C는 WHATWG와 공동으로 HTML5 제정에 합류하여 2008년 HTML 5 초안 공개. 2009년 7월 XHTML 2.0의 개발은 중지됨. ![HTML의 역사](https://t1.daumcdn.net/cfile/tistory/120BBC3D50B2419637)

  8. 2012년 이후 W3C의 표준과 WHATWG의 서로 다른 설계로 인해 표준이 점차 다양해짐. 그러다 2019년 5월 28일 W3C는 WHATWG가 HTML 및 DOM 표준의 유일한 게시자가 될 것이라고 발표. WHATWG "Living Standard"는 한동안 de facto가 됨.

  - HTML 표준을 지키는 것은 왜 중요할까요?
  - XHTML 2.0은 왜 세상에 나오지 못하게 되었을까요?
  - HTML5 표준은 어떤 과정을 통해 정해질까요?

- 브라우저의 역사는 어떻게 될까요?
  - Internet Explorer가 브라우저 시장을 독점하면서 어떤 문제가 일어났고, 이 문제는 어떻게 해결되었을까요?
  - 현재 시점에 브라우저별 점유율은 어떻게 될까요? 이 브라우저별 점유율을 알아보는 것은 왜 중요할까요?
  - 브라우저 엔진(렌더링 엔진)이란 무엇일까요? 어떤 브라우저들이 어떤 엔진을 쓸까요?
  - 모바일 시대 이후, 최근에 출시된 브라우저들은 어떤 특징을 가지고 있을까요?
- HTML 문서는 어떤 구조로 이루어져 있나요?
  - `<head>`에 자주 들어가는 엘리먼트들은 어떤 것이 있고, 어떤 역할을 할까요?
  - 시맨틱 태그는 무엇일까요?
    - 시맨틱 엘리먼트를 사용하면 어떤 점이 좋을까요?
    - `<section>`과 `<div>`, `<header>`, `<footer>`, `<article>` 엘리먼트의 차이점은 무엇인가요?
  - 블록 레벨 엘리먼트와 인라인 엘리먼트는 어떤 차이가 있을까요?

## Quest

- [이 화면](screen.png)의 정보를 HTML 문서로 표현해 보세요. 다만 CSS를 전혀 사용하지 않고, 문서의 구조가 어떻게 되어 있는지를 파악하여 구현해 보세요.
  - [CSS Naked Day](https://css-naked-day.github.io/)는 매년 4월 9일에 CSS 없는 웹 페이지를 공개하여 내용과 마크업에 집중한 HTML 구조의 중요성을 강조하는 행사입니다.
- 폴더에 있는 `skeleton.html` 파일을 바탕으로 작업해 보시면 됩니다.
  - 화면을 구성하는 큰 요소들을 어떻게 처리하면 좋을까요?
  - HTML 문서상에서 같은 층위에 비슷한 요소들이 반복될 때는 어떤 식으로 처리하는 것이 좋을까요?

## Advanced

- XML은 어떤 표준일까요? 어떤 식으로 발전해 왔을까요?
- YML, Markdown 등 다른 마크업 언어들은 어떤 특징을 가지고 있고, 어떤 용도로 쓰일까요?

## References

- https://en.wikipedia.org/wiki/HTML
- https://hyoje420.tistory.com/22
