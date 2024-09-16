#### The Mechanics of start in react
How is a component view is update then ?
- Basic react principles is re-rendering the component , which is call back the component again.
- But now in react without re-rendering the whole page we can change the state of the component. 
- that why we need use state.
### Controlled elements
- Create piece of state.
- Define piece of state.
- Set function for the changing the state.  

```
function Counter() {

const [count, setCount] = useState(0)

const [step, setStep] = useState(1)

  

const date = new Date("September 10 2024")

date.setDate(date.getDate() + count)


return (

<div>

<div>

<button onClick={() => setStep((s) => s - 1)}>-</button>

<span>Step : {step}</span>

<button onClick={() => setStep((s) => s + 1)}>+</button>

</div>

<div>

<button onClick={() => setCount((c) => c - step)}>-</button>

<span>Count: {count}</span>

<button onClick={() => setCount((c) => c + step)}>+</button>

</div>

<p>

{date.toDateString()}

</p>

</div>

)

}
```

The above code snippet is example for controlled element.