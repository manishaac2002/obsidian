![[state.png]]

### Controlled elements
- Create piece of state.
- Define piece of state variable.
- Set function where state is updating.


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