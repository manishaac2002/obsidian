![[child prop.png]]

Why and When we are using child props?
     We cant use props for each component differently for specific reason, In case 
    in need of two button we need one set props for one button and another set of props for another button button. So in this case we can use it as ==child props==.
    
```
<Button bgColor={'#7950f2'}

textColor={'white'}

onClick={handlePrevious}>

<span>👈</span> Previous

</Button>       

<Button bgColor={'#7950f2'}

textColor={'white'}

onClick={handleNext}>

Next <span>👉</span>

</Button>
```


Look at this above button emojis its difficult while using the normal form of props, instead props we are using child props.


```
 function Button({ textColor, bgColor, onClick, children }) {

return (

<button style={{ background: bgColor, color: textColor }}

onClick={onClick}>

{children}

</button>

)

}

}
```

Child component for button  component, passing the child prop into it.




