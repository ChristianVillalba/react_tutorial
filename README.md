# React Tutorial
Notes to Setup our Local Environment for creating React Apps     

## Description

Setting up our environment and displaying     
A simple Hello World       
Instructor: Dr. Angela Yu     


## Getting Started

### Dependencies

* Visual Studio Code (+Extensions):     
    * Babel JavaScript    
    * VScode-icons     
* Node

### Installing

* Check Node is Up to Date:
    * Check my Node version using:    
    ```
    node --version
    ```
    * Compare with the latest Node Version:     
    [NODE JS](https://nodejs.org/en/)
* Create React App     
    ```
    npx create-react-app my-app
    ```
* Run React App 
    ```
    cd my-app    
    npm start
    ```

## Hello World: Introduction to React
* index.html:  
 
```
...
<body>
  <div id="root"></div>
  <script>src="./src/index.js" type="text/jsx"</script>
</body>
```  
To be able to use React,      
We need to create, in our index.html file, a div with the id="root"     
This is the root of our React Application     
Everything created with React will be inserted in this div.

The script in our HTML file that links to our JS file, must be changed: type= from javascript to JSX 


The HTML file won't be used anymore,     
all the code is written in the JS file (index.js) using JS and React
   
* index.js:     
```
import React from 'react';
import ReactDOM from 'react-dom';
ReactDOM.render(
  <h1>Hello World</h1>,
  document.getElementById('root')
);
```  
In our JS file (index.js by convention):        
The first step will be to import React and ReactDom modules      

Now we can use both packages:      
ReactDom.render() takes 2 inputs:      
* Input 1: What to show
* Input 2: Where to show
* Input 3 (optional) : callback function whnt render is complieted  
   
We placed an H1 Element (what) inside our div id="root" (where)      
React creates this as a JSX file, 
this way index.js knows that is HTML and not JS.   

   

## Babel
Our HTML is compiled by the React modeule     
Babel (JS Compiler) takes modern JS (JSX in this case)      
and compile it down to a version of JS that any browser can understand
This solves problems about browser compatibilities       
