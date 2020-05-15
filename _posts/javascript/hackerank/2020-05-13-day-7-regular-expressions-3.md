---
layout:            post
title:             "Regular Expressions 3"
menutitle:         "Regular Expressions 3"
date:              2020-05-13 13:30:00 +0900
tags:              Javascript HackerRank
category:          Javascript
author:            charllossDev
cover:             /assets/mountain-alternative-cover.jpg
published:         true
redirect_from:     "/Regular-Expressions-3-Redirect/"
cover:             /assets/mountain-alternative-cover.jpg
language:          EN
comments:          true
math:			   false
---

# Regular Expressions 3

### Task

Complete the function in the editor below by returning a RegExp object, , that matches every integer in some string .

### Constraints

The length of string  is  .
It's guaranteed that string  contains at least one integer.

### Output Format

The function must return a RegExp object that matches every integer in some string .

### Sample Input 0
```
102, 1948948 and 1.3 and 4.5
```
### Sample Output 0

```
102
1948948
1
3
4
5
```

### Explanation 0

When we call match on string  and pass the correct RegExp as our argument, it returns the following
array of results: [ '102', '1948948', '1', '3', '4', '5' ].

# Dev

```js
'use strict';

process.stdin.resume();
process.stdin.setEncoding('utf-8');

let inputString = '';
let currentLine = 0;

process.stdin.on('data', inputStdin => {
    inputString += inputStdin;
});

process.stdin.on('end', _ => {
    inputString = inputString.trim().split('\n').map(string => {
        return string.trim();
    });

    main();    
});

function readLine() {
    return inputString[currentLine++];
}

function regexVar() {
    /*
     * Declare a RegExp object variable named 're'
     * It must match ALL occurrences of numbers in a string.
     */

    const re = /\d+/g;
    /*
     * Do not remove the return statement
     */
    return re;
}
```
