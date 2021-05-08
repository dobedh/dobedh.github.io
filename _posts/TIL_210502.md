---
title: TIL_210502
date: 2021-05-02
tags:
  - React
  - jsx
---

### Component

- react는 Component를 가져와서 브라우져가 이해할 수 있는 html로 변환해준
- 이떄, react가 html로 반환하는 모든 것들을 componenet라고 부름

### JSX

- Javascript + HTML = JSX

### Component 만드는 법

- Upper Case로 시작하는 function을 만든다

```
function Potation() {
    return
}
```

### React app은 하나의 Componennt만 렌더할 수 있다

- 따라서 다양한 component를 기본 component 안에 집어 넣어서(중첩으로) 사용한다.

### Property (props)

- JSX에서는, 각 component에 props 값을 부여해서, 각 componenet에 전달할 수 가 있다.
- 예를 들어, fav=kimchi라는 것을 componenet값으로 전달 할 수 있는 것

### Map

- JS 언어로, array에 있는 각 요소들에 func을 걸수 있도록 함

```
function App() {
  return foodILike.map((dish) => {
    return <Food name={dish.name} picture={dish.image} />;
  });
}
```

### Prop-Types

- Component에서 전달하는 Prop이 적절한 type인지, required 인데 전달이 안됐는지 등을 체크해준다.
- npm i prop-types
- import PropTypes from "prop-types"

```
Food.propTypes = {
  name: PropTypes.string.isRequired,
  picture: PropTypes.string.isRequired,
  rating: PropTypes.number,
};
```
