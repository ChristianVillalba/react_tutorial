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

### Hello World:
* index.html:   
    ```
    <body>
      <script>src="./src/index.js" type="text/jsx"</script>
      <div id="root"></div>
    </body>
    ```  
   
* index.js:     
    ```
    import React from 'react';
    import ReactDOM from 'react-dom';
    ReactDOM.render(
      <h1>Hello World</h1>,
      document.getElementById('root')
     );
    ```  
   

