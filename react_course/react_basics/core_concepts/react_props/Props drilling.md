What is props drilling 
Disadvantage of using props drilling
Why we go for component composition
#### **What is props drilling** 
**Props drilling** refers to the process of passing data from a parent component to deeply nested child components through multiple layers of intermediate components

```
function Parent() {
  const data = "Hello from Parent!";
  return <Child data={data} />;
}

function Child({ data }) {
  return <GrandChild data={data} />;
}

function GrandChild({ data }) {
  return <p>{data}</p>;
}
```
Above code snippet , the data is prop drilling which is passing props passes to the grand child( i.e deeply nested child component).

#### **Disadvantage of using props drilling**
- When we pass props to grandchild is more difficult to pass like this in huge react project.
- It may confuse to developer too because if there is many props to pass like this as nested child component.
- Instead we can use [[Components composition]].