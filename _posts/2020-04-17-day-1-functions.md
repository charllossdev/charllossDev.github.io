---
layout:            post
title:             "Functions"
menutitle:         "Functions"
date:              2020-04-17 16:00:00 +0900
tags:              Javascript HackerRank
category:          Javascript
author:            charllossDev
cover:             /assets/mountain-alternative-cover.jpg
published:         true
redirect_from:     "/Functions-Redirect/"
cover:             /assets/mountain-alternative-cover.jpg
language:          EN
comments:          true
math:			   false
---

# Functions

## Task

Implement a function named factorial that has one parameter: an integer $n$. It must return the value of $n!$ (i.e., $n$ factorial).

## Input Format

Locked stub code in the editor reads a single integer, $n$, from stdin and passes it to a function named factorial.

## Constraints

$ 1 < n < 10 $

## Output Format

The funciton must return the value of $n!$.

# Input
```js
4
```

# Output
```js
24
```

# Explanation
we return the value of $4! = 4 * 3 * 2 * 1 = 24$

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
/*
 * Create the function factorial here
 */

function factorial(n) {

    let i, result = n;

    for (i = n -1; i >= 1; i--) {
        result *= i;
    }

    return result;
}


function main() {
    const n = +(readLine());

    console.log(factorial(n));
}
```
