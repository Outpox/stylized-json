I needed a *npm package* version of this [snippet](http://jsfiddle.net/unLSJ/) so I created it. Although please note that I'm not the author of the script itself.  
The goal of this package is to display a JS object like: ![](http://i.imgur.com/mFN432Y.png)  
  
###Installation:  
`npm install stylized-json`  

Don't forget to include the css file if needed like:  
`<link rel="stylesheet" href="node_modules/stylized-json/index.css">`
  
##Usage:
```javascript
import stylizedJson from 'stylized-json';

let myObj = {test: {fr_FR: "test", en_US: "test"}},
    myObjToHtml = stylizedJson.prettyPrint(myObj);
    
document.body.innerHTML += myObjToHtml;
```