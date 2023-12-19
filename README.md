"# chand" 

This repository is created for giving demo on git & git hub

things i did for making this repository

+ Created a empty repository named `chandru`
* this link is open to git hub (https://github.com/Chandruvijayakumar/chand).
```
// Getting input via STDIN
const readline = require("readline");

const inp = readline.createInterface({
  input: process.stdin
});

const userInput = [];

inp.on("line", (data) => {
  userInput.push(data);
});

inp.on("close", () => {
  // Your code logic goes here
  const monthNumber = parseInt(userInput[0]);

  function daysInMonth(monthNumber) {
    if (1 <= monthNumber && monthNumber <= 12) {
        // 30 days for April, June, September, and November
        if ([4, 6, 9, 11].includes(monthNumber)) {
            return 30;
        }
        // 31 days for January, March, May, July, August, October, and December
        else if ([1, 3, 5, 7, 8, 10, 12].includes(monthNumber)) {
            return 31;
        }
        // 28 days for February
        else {
            return 28;
        }
    } else {
        return "Error";
    }
  }

  // Calculate and print the result
  const result = daysInMonth(monthNumber);
  console.log(result);
});
```

