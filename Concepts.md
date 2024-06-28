```javascript
// var React = require("react");
import React from "react"; // better way
// var ReactDOM = require("react-dom");
import ReactDOM from "react-dom";

// This is how long it takes to write Hello World using pure JS
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
//-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
// ATTRIBUTES
const img = "https://picsum.photos/200";
reactDom.render(
  <div>
    <h1 contentEditable="true" spellCheck="false">
      My favourite food
    </h1>
    <img
      src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRIqQj7_XYNe9u-w6IOyVyR5KXUo7DI2US_vw&s"
      alt="Ramyeon"
    />
    <img
      src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQHVE61TcD04Sxjadcu68idNbC13y1Sw3PUtw&s"
      alt="Takoyaki"
    />
    <img
      src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSwTu9QjEDUIJsXUf8EYbdHVX39tBFl8WgSJg&s"
      alt="full Plate"
    />
    <img src={img} alt="random" />
  </div>,
  document.getElementById("root")
);

// Generally, we write the whole HTML global attributes in lowercase but when it comes to be write HTML attributes in JSX we write in camelcase otherwise it'll not work.
// e.g. contenteditable="true" in HTML file, but contentEditable="true" in JSX file.


```
