# Quest 02. CSS의 기초와 응용

## Introduction

- CSS는 Cascading StyleSheet의 약자입니다. 웹브라우저에 표시되는 HTML 문서의 스타일을 지정하는 (거의) 유일하지만 다루기 쉽지 않은 언어입니다. 이번 퀘스트를 통해 CSS의 기초적인 레이아웃 작성법을 알아볼 예정입니다.

## Topics

- CSS의 기초 문법과 적용 방법
  - Inline, `<style>`, `<link rel="stylesheet" href="...">`
- CSS 규칙의 우선순위
- 박스 모델과 레이아웃 요소
  - 박스 모델: `width`, `height`, `margin`, `padding`, `border`, `box-sizing`
  - `position`, `left`, `top`, `display`
  - CSS Flexbox와 Grid
- CSS 표준의 역사
- 브라우저별 Developer tools

## Resources

- [MDN - CSS](https://developer.mozilla.org/ko/docs/Web/CSS)
- [Centering in CSS: A Complete Guide](https://css-tricks.com/centering-css-complete-guide/)
- [A complete guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
- [그리드 레이아웃과 다른 레이아웃 방법과의 관계](https://developer.mozilla.org/ko/docs/Web/CSS/CSS_Grid_Layout/%EA%B7%B8%EB%A6%AC%EB%93%9C_%EB%A0%88%EC%9D%B4%EC%95%84%EC%9B%83%EA%B3%BC_%EB%8B%A4%EB%A5%B8_%EB%A0%88%EC%9D%B4%EC%95%84%EC%9B%83_%EB%B0%A9%EB%B2%95%EA%B3%BC%EC%9D%98_%EA%B4%80%EA%B3%84)

## Checklist

- **CSS를 HTML에 적용하는 세 가지 방법은 무엇일까요?**

  CSS를 적용하는 3가지 방법으로 **inline, internal, external CSS**가 있다.

  1. **inline CSS**
     HTML의 `style` attribute에 CSS를 기술하는 방법이다. 특정 HTML element를 대상으로만 스타일을 입힐 수 있다.

     ```HTML
     <p style="color: blue;">This is a paragraph.</p>
     ```

  2. **internal CSS**
     HTML의 `<head>` 태그 사이에 `<style>` 태그를 삽입하여 전체 HTML에 대해 CSS를 적용하는 방법이다.

     ```HTML
     <head>
        <style>
           h1 {
              color: red;
              margin-left: 20px;
           }
        </style>
     </head>
     ```

  3. **external CSS**
     CSS를 `.css` 확장자의 파일로 분리하여 `<head>` 태그 사이에 `<link>` 태그를 삽입하여 HTML에 CSS를 적용하는 방법이다.

     ```HTML
     <link href="style.css" rel="stylesheet" type="text/css">
     ```

- **세 가지 방법 각각의 장단점은 무엇일까요?**

  1. **inline CSS**

  - **Pros**: 빠르게 프로토타이핑/수정하는데 유용하며 `.css` 파일로의 switch 없이 CSS를 작성할 수 있다는 점에서 코드 작성이 수월하다. 또한 대부분의 email client는 `.css`를 불러오는 것을 허용하지 않기 때문에(스팸의 가능성으로 보고), inline style을 사용해야 한다.
  - **Cons**: HTML에 CSS가 포함되기 때문에 HTML을 불러올 때 그만큼 더 많은 bandwidth를 사용한다. inline으로 작성된 CSS는 재사용이 불가능하다.

  2. **internal CSS**

  - **Pros**: inline CSS와 동일하게 수정이 용이하다. 또 나중에 external CSS로 분리할 때 편리하다는 장점이 있다.
  - **Cons**: inline CSS와 동일하게 HTML의 양이 늘어나고, 특정 email client에서는 `head` 부분이 제거될 수 있어서 주의해야 한다.

  3. **external CSS**

  - **Pros**: 유지 보수가 쉽고 페이지 간 CSS 재사용이 가능하다. 또 `.css` 파일은 캐싱이 가능해서 bandwidth를 적게 사용할 수 있고, 웹 서버의 요청 부담을 줄이며 페이지 로드 속도를 높일 수 있다. 또 HTML과 분리되기 때문에 unused CSS를 제거할 수 있다.

  - **Cons**: email client에서는 거의 사용할 수 없다. 파일 별로 부가적인 HTTP 요청을 날리기 때문에 라우터/방화벽 단의 리소스 사용률이 높아진다.

- CSS 규칙의 우선순위는 어떻게 결정될까요?
- CSS의 박스모델은 무엇일까요? 박스가 화면에서 차지하는 크기는 어떻게 결정될까요?
- `float` 속성은 왜 좋지 않을까요?
- Flexbox(Flexible box)와 CSS Grid의 차이와 장단점은 무엇일까요?
- CSS의 비슷한 요소들을 어떤 식으로 정리할 수 있을까요?

## Quest

- Quest 01에서 만들었던 HTML을 바탕으로, [이 그림](screen.png)의 레이아웃과 CSS를 최대한 비슷하게 흉내내 보세요. 꼭 완벽히 정확할 필요는 없으나 align 등의 속성은 일치해야 합니다.
- **주의사항: 되도록이면 원래 페이지의 CSS를 참고하지 말고 아무것도 없는 백지에서 시작해 보도록 노력해 보세요!**

## Advanced

- 왜 CSS는 어려울까요?
- CSS의 어려움을 극복하기 위해 어떤 방법들이 제시되고 나왔을까요?
- CSS가 브라우저에 의해 해석되고 적용되기까지 내부적으로 어떤 과정을 거칠까요?
- 웹 폰트의 경우에는 브라우저 엔진 별로 어떤 과정을 통해 렌더링 될까요?

```

```
