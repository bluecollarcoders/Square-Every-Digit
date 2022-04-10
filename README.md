# Square-Every-Digit

## Problem 
Description:
Welcome. In this kata, you are asked to square every digit of a number and concatenate them.

For example, if we run 9119 through the function, 811181 will come out, because 92 is 81 and 12 is 1.

Note: The function accepts an integer and returns an integer

## Solution 1
```javascript
const squareDigits= (num) => {
// convert parameter to string
  var numString = num.toString();
// create empty string to store number strings
  var sum = "";
// run for loop
for(let i in numString ) {
  sum += (parseInt(numString[i])**2 + "");
}
  return parseInt(sum);
}
```

## Solution 2
```javascript
function squareDigits(num){
  var stringNum = num.toString();
  var sum = [];
  
  for(let i = 0; i < stringNum.length; i++) {
    sum[i] = stringNum[i] * stringNum[i]
  }
  return Number(sum.join(''));
}
```
