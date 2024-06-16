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
```
