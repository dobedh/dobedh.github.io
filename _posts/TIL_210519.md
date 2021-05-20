---
title: TIL-210519
date: 2021-05-19
tags:
  - react
  - Hooks
  - useTabs
---

# Hooks

### useTabs

- useState를 활용한 예제 연습중..

```
    const useTabs = (initialTab, allTab) => {
      const [tab, setTab] = useState(initialTab);
      const onClick = (allTab) => {
        return console.log(allTab);
      };
      return onClick;
    };

    const content = [
      {
        item: "item1",
        content: "this is the name of item 1"
      },
      {
        item: "item2",
        content: "this is the name of item 2"
      }
    ];

    const App = () => {
      const tabs = useTabs(0, getIndex);
      const getIndex = (index) => {
        return index;
      };
      return (
        <div className="App">
          {content.map((section) => {
            return <button onClick={getIndex}> {section.item}</button>;
          })}
        </div>
      );
    };
```
