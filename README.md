# Simple-Number-Guessing-Game-Using-Javascript
This is a small game using javascript.

### Here is the code 
---
```Js
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>
  <body>
    <h1 class="guessingGame">Let's Play Number guessing Game</h1>
    <script>
      // make a number guessing game

      var randNum = Math.floor(Math.random() * 100) + 1;
      let guess = 0;

      let flag = true;
      let guessNum = window.prompt("Enter a Number : ");
      while (flag) {
        if (guessNum == randNum) {
          flag = false;
          continue;
        } else if (guessNum > randNum) {
          console.log("Guess a small number");
          guessNum = window.prompt("Enter a small Number : ");
        } else {
          console.log("Guess a large number");
          guessNum = window.prompt("Enter a large Number : ");
        }

        guess++;
      }

      console.log(`you took ${guess} guess to reach correct number`);
      console.log(`Thanks for playing This Game`);
    </script>
  </body>
</html>
```
