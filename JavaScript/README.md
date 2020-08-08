***We have a client/user that sends an HTTP Request to a server, which sends back an HTTP Response. All of the Python code we’ve written so far using Django has been running on a server. JavaScript will allow us to run code on the client side, meaning no interaction with the server is necessary while it’s running, allowing our websites to become much more interactive.***

```javascript
let counter = 0;
function count() {
  counter++;
  document.querySelector('h1').innerHTML = counter;
}  
```

**Events**  
One feature of JavaScript that makes it helpful for web programming is that it supports Event-Driven Programming.  
***Event-Driven Programming*** ( is a programming paradigm that centers around the detection of events, and actions that should be taken when an event is detected.  

The idea of DOM manipulation to improve our counter page:  

```javascript
let counter = 0;
            function count() {
                counter++;
                document.querySelector('h1').innerHTML = counter;
            }
```
```
<button onclick="count()">Count</button>
```

We can make this page even more interesting by displaying an alert every time the counter gets to a multiple of ten. In this alert, we’ll want to format a string to customize the message, which in JavaScript we can do using **template literals**. Template literals require that there are backticks () around the entire expression and a $ and curly braces around any substitutions.  
```javascript
function count() {
    counter++;
    document.querySelector('h1').innerHTML = counter;
    
    if (counter % 10 === 0) {
        alert(`Count is now ${counter}`)
    }
}
```
