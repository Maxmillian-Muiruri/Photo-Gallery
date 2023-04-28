## PHOTOGALLERY PROJECT

- forEach
- styling using javascript
- using inner.HTML
- using innerText
- what is .then in javascript
- how to use addEventListener
- how Math.random is used

## using for each

### It is mainly used to traverse the array or collection elements

### Javascript For-each Loop

```const numbers = [65, 44, 12, 4];
numbers.forEach(myFunction)

function myFunction(item, index, arr) {
  arr[index] = item * 10;
}
```

# styling using javascript

### The HTML DOM allows JavaScript to change the style of HTML elements.

### To change the style of an HTML element you use this

```
document.getElementById(id).style.property = new style
```

### The following example changes the style color of a <p> element:

```js
document.getElementById("p2").style.color = "blue";
</script>
```

## using inner.HTML

## The innerHTML property sets or returns the HTML content (inner HTML) of an element.

### The innerHTML property returns:The text content of the element, including all spacing and inner HTML tags.

### example

```
Change the HTML content of an element with id="demo":

document.getElementById("demo").innerHTML = "I have changed!";
```

# using innerText

## HTML DOM Element innerText

### The innerText property sets or returns the text content of an element.

### The innerText property returns:Just the text content of the element and all its children, without CSS hidden text spacing and tags, except `<script> and <style>` elements.

### example

```
let text = document.getElementById("myP").innerText;
```

# what is .then in javascript

## The then() method in JavaScript has been defined in the Promise API and is used to deal with asynchronous tasks such as an API call.

### example

```
function demo() {
    console.log("Function called!!")
    return Promise.resolve("Success");
    // or
    // return Promise.reject("Failure");
}
demo().then(
    (message) => {
        console.log("Then success:" + message);
    }
)

Output:

Function called!!
Then success:Success
```

## Using then() as an asynchronous function

```
var demo = new Promise((resolve, reject) => {
    resolve(1);
})
let call = demo.then(
    (value) => {
        console.log(value);
        return ++value;
    },
    (message) => {
        console.log(message);
    });
    console.log(call);
    setTimeout(() => {
    console.log(call);
});


Output:

Promise {status: "pending"}
1
Promise {status: "resolved", result: 2}
```

## how to use addEventListener

### An event listener is a procedure in JavaScript that waits for an event to occur.

### The addEventListener() is an inbuilt function in JavaScript which takes the event to listen for, and a second argument to be called whenever the described event gets fired

### The addEventListener() method makes it easier to control how the event reacts to bubbling.

### When using the `addEventListener() `method, the JavaScript is separated from the HTML markup, for better readability and allows you to add event listeners even when you do not control the HTML markup

### Example

### Alert "Hello World!" when the user clicks on an element:

```
element.addEventListener("click", myFunction);

function myFunction() {
  alert ("Hello World!");
}
```

### The first parameter is the type of the event (like "click" or "mousedown" or any other HTML DOM Event.)

### The second parameter is the function we want to call when the event occurs.

### The third parameter is a boolean value specifying whether to use event bubbling or event capturing. This parameter is optional.

# how Math.random is used

## JavaScript Math.random()

### The Math. random() method returns a random number from 0 (inclusive) up to but not including 1 (exclusive)

### example

```
function getRandomInt(max) {
  return Math.floor(Math.random() * max);
}

console.log(getRandomInt(3));
// Expected output: 0, 1 or 2

console.log(getRandomInt(1));
// Expected output: 0

console.log(Math.random());
// Expected output: a number from 0 to <1

```
