# Event-driven programming with typing game


I'm afraid you will confused this evnet driven programming term with earlier explanined object oriented programming and functional programming.

OOP and FP are essential a way to abstract, organize our program for cleaner view for either developers or computer.

For example, When we think about a Person, we could think of many things to construct a person, his name, age, height, sex, interest, etc. If we have over hundred person, and we do not organize the person, the code will get really messy. That is when OOP shine, where we can create a Person class, and create hundred and thounsands of person.

Where event driven programming is a trival ideas of, we will run specific programming only when somthing (event) happen. That something (event) might be when a user click a bottom, or hover around a link, or select some of the text.

```
Event : something which happen   ` Merriam-Webster`
```

In the earlier day, Javascript was invented for form validations.

Picture show how communication between server and client take longer time than today.

So, javascript was used to do simple form validation like, if the phone number is correct ? are the user name okie? is the password too long or too short? etc.

javascript will make sure to submit the form only after the validation is done. and when click the submit bottom, an submit event is triggered.



Event driven is not like our usually written programming.

Let's review our typical functions, which is called the procedural programming.

```javascript
// Define a function
const gretting = (name, age) => {
  console.log(f`Hello, ${name} you are ${age} years old`)
}


// Call a function
gretting('Curry', '30')
gretting('James', '23')

// Out
// Hello, Curry you are 30 years old
// Hello, James you are 23 years old
```

In procedual programming, the programming is run in a specific order. typically from top to botton, if we add timeout or such, it will store in call stack and run in a specific order.

When we add the above concepts with event, it would be saying, hey, I want you to call the function only after some conditions ( event ) have fullfilled.

## Event Listener

To handle events (button clicking, typing, etc.), we register **event listeners**. An event listener is a function which listens for an event to occur and executes in response. Event listeners can update the UI, make calls to the server, or whatever else needs to be done in response to the user's action. We add an event listener by using [addEventListener](https://developer.mozilla.org/docs/Web/API/EventTarget/addEventListener), and providing a function to execute.


### Common events

- click
- contextMenu
- select
- input
