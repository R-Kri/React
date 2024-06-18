```  javascript

// Inline styling in JSX
const customStyleHead = {
  color: "blue",
  fontSize: "34px",
  border: "3px solid black",
};
const customStylePara = {
  color: "rgb(32,224,123)",
  fontSize: "18px",
  border: "1px solid yellow",
  padding: "30px",
};

// Biggest advantage of inline styling is easy updation.
customStyleHead.color = "orange";

reactDom.render(
  <div>
    <h1 style={customStyleHead}>Hey there!</h1>
    <p style={customStylePara}>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Tempora vitae
      debitis impedit fugiat suscipit? Sapiente, illum libero ea, repellat
      labore facilis neque, voluptate soluta expedita asperiores eum sunt
      deserunt odit.
    </p>
  </div>,
  document.getElementById("root")
);

```
