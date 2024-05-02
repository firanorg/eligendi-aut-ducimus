<div align="center">
 <h1> <img src="https://github.com/firanorg/eligendi-aut-ducimus/assets/81325730/fb8c8369-e2c9-473f-8493-542fafdbfecc" width="80px"><br/>PDF Parser Client Side</h1>
 <a href="https://itsvg.in" target="_blank"><img src="https://img.shields.io/badge/Creator-Vishwa%20Gaurav-blue"/></a> 
 <img src="https://img.shields.io/npm/v/@firanorg/eligendi-aut-ducimus?label=%20"/>
 <img src="https://img.shields.io/npm/dt/@firanorg/eligendi-aut-ducimus">
 <img src="https://img.shields.io/snyk/vulnerabilities/github/VishwaGauravIn/@firanorg/eligendi-aut-ducimus"/>
 <img src="https://img.shields.io/badge/License-MIT-brightgreen"/>
 <img src="https://img.shields.io/github/languages/code-size/VishwaGauravIn/@firanorg/eligendi-aut-ducimus?logo=github">
</div>

## PDF Parser Client Side
A lightweight easy to use package to parse text from PDF files on client side without any server dependency.

## How to Install ?
Use npm or yarn to install this npm package

```js
npm i @firanorg/eligendi-aut-ducimus
```
or
```js
yarn add @firanorg/eligendi-aut-ducimus
```

Include the package

```js
import extractTextFromPDF from "@firanorg/eligendi-aut-ducimus";
```

Basic Example:

```jsx
import React from "react";
import extractTextFromPDF from "@firanorg/eligendi-aut-ducimus";

export default function Test() {
  return (
    <div>
      <input
        type="file"
        name=""
        id="file-selector"
        accept=".pdf"
        onChange={(e) => {
          // Selecting the first file
          const file = e.target.files[0];
          //   If file exists then we will call our function
          if (file) {
            extractTextFromPDF(file).then((data) => {
              console.log(data);
            });
          }
        }}
      />
    </div>
  );
}

```

## Contributing

Feel free to contribute!

1. Fork the repository
2. Make changes
3. Submit a pull request

### [</> with 💛 by Vishwa Gaurav](https://itsvg.in)
