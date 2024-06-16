```javascript
// var React = require("react");
import React from "react"; // better way
// var ReactDOM = require("react-dom");
import ReactDOM from "react-dom";

// This is how it long it takes to write in pure JS
// var h1 = document.createElement("h1");
// h1.innerHTML = "Hello World";
// document.getElementById("root").appendChild(h1);

// NOTE: ReactDOM.render(What to show, where to show it);

ReactDOM.render(
  <div>
    <h1> Hello World!</h1>
    <p>How are you?</p>
  </div>,
  document.getElementById("root")
);
/*
render method takes only a single HTML element.
Anything goes inside a div also counts as a single element. But can have many child element.
*/
ReactDOM.render(
  <div>
    <h1>Hey</h1>
    <ul>
      <li>jj</li>
      <li>mj</li>
      <li>pk</li>
    </ul>
  </div>,
  document.getElementById("root")
);


/*
As JSX allows us to insert html in JS, further more it also allows us to insert 
js under html.
*/
const name = "Angela";
const Lastname = "Yu";
const num = 13;

// You can add any JS expression between those curly braces. But we can't write JS statements like conditionals
ReactDOM.render(
  <div>
    <h1>Hello {name + " " + Lastname}!</h1>
    <h1>
      Hello {name} {Lastname}!
    </h1>
    <h1>Hello {`${name} ${Lastname}`}!</h1>
    <p>My lucky number is {Math.floor(Math.random() * 10)}</p>
  </div>,
  /* 
3rd method is called Template literal or string interpolation method but very comple at the situation to use.
*/
  document.getElementById("root")
);

```
