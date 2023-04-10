## Webpack switching between watch and dev server issue

Steps to reproduce:
1. `npm install`
2. `npm run dev` and wait 10s or until node_modules/.cache folder appear/update
3. `npm run watch` open dist/index.html and look at browser console

You will see 
>Uncaught TypeError: Cannot read properties of undefined (reading 'dispose')
at eval (index.css:7:18)
at ./index.css (main.js:49:1)
at __webpack_require__ (main.js:73:41)
at eval (index.js:2:68)
at ./index.js (main.js:19:1)
at __webpack_require__ (main.js:73:41)
at main.js:96:37
at main.js:98:12