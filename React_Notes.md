# What is React?
- React is a JavaScript library that efficiently renders the UI of web applications
# What does it do?
## Utilizes JSX
- JSX is a convenient tool to write readable HTML within JavaScript e.g `{/*this is JS inside JSX*/}`
- JSX is not valid JavaScript and therefore must be compiled into JavaScript with the Babel transpiler
- JSX must return a single html element which may have nested elements within it e.g :
```
const JSX = (
<div>
  <p> One P element </p>
  <p> One P element </p>
</div>
);
```
- JSX uses camelcase for html attributes and events e.g `class` -> `className`, `onclick` -> `onClick`
- Any JSX element can be self closing e.g `<div></div>` -> `<div />` however, single tag elements must be self closing e.g `<br>` -> `<br />`
## React DOM
- the HTML DOM model is the tree structure of html elements
- When the state of a webpage is changed, the DOM must be updated and re-rendered to reflect the new state. Related operations can be expensive.
- React offers a less expensive method of updating the DOM via use of the 'Virtual DOM'
- React stores an 'old state' DOM and a 'new state' DOM in memory & uses a diffing algorithm to determin an efficient way to update the actual DOM
- JSX is rendered to the DOM with `ReactDOM.render(componentToRender, targetNode)` e.g `ReactDOM.render(JSX, document.getElementById('root'))`
- Creates two virtual trees and Compares them, keys help with this diff algorithm
- Uses a diffing algorithm to calculate minimum operations to patch only the 
- The HTML DOM https://www.w3schools.com/whatis/whatis_htmldom.asp
- Tech Talk: What is the Virtual DOM?: https://www.youtube.com/watch?v=d7pyEDqBDeE 
## create components
- Components are the core of React
- Components in React can either be stateless functional components or ES6 class components
- a stateless functional component can receives data and it returns JSX
## handle state
## handle props
## utilize event listeners
## utilize certain life cycle methods to update data as it changes
