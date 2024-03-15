<div align="center">
  <br/>
  <h1> <b> Task2.1P </b></h1>
</div>
<p align="center">
  <img alt="NPM Version" src="https://img.shields.io/badge/npm-10.1.0-red">
  <img alt="NODE Version" src="https://img.shields.io/badge/NodeJS-20.9.0-green">
</p>

### Project initialization
Use the following command in Terminal to initialize the project files. This step is to install the necessary dependencies required for the Node execution environment.
``` bash
npm init -y
```

### Explanation of code
``` js
const express = require('express');
const app = express();
```
These two lines of code first introduce the express framework, and then instantiate the express framework to reference its methods.

``` js
app.listen(port, () => {
    console.log(`Server is running on port ${port}`);
});
```
This line of code calls the ``listen`` method in the express framework, which uses the port variable we previously defined to occupy port 3000 and provide web service.

``` js
app.get('/', (req, res) => {
    res.send(`<h1>Hello World</h1>`);
});
```
This line of code is responsible for routing user access to the corresponding content. When the user visits the root directory of the webpage, the "Hello World>" is returned to the user, and the browser will render this HTML code to the corresponding style.

### Run the project
Use the following command to run this project
``` bash
node app.js
```
