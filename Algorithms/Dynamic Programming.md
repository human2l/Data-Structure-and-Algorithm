Dynamic Programming is just using cash/memoization to optimizing the code. just a buzzword

# Memoization

<img src="Dynamic Programming.assets/Screen Shot 2022-02-04 at 6.15.21 PM.png" alt="Screen Shot 2022-02-04 at 6.15.21 PM" style="zoom:25%;" />

Note: using closure

<img src="Dynamic Programming.assets/Screen Shot 2022-02-04 at 7.14.36 PM.png" alt="Screen Shot 2022-02-04 at 7.14.36 PM" style="zoom:50%;" />

<img src="Dynamic Programming.assets/Screen Shot 2022-02-04 at 7.15.04 PM.png" alt="Screen Shot 2022-02-04 at 7.15.04 PM" style="zoom:50%;" />

# Bottom-up

Memoization -- fibonacciMaster()

Bottom-up -- fibonacciMaster2()

```js
//0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89, 144, 233...
let calculations = 0;
function fibonacci(n) { //O(2^n)
  
  if (n < 2) {
    return n
  }
  return fibonacci(n-1) + fibonacci(n-2);
}

function fibonacciMaster() { //O(n)
  let cache = {};
  return function fib(n) {
    calculations++;
    if (n in cache) {
      return cache[n];
    } else {
      if (n < 2) {
        return n;
      } else {
        cache[n] = fib(n-1) + fib(n-2);
        return cache[n];
      }
    }
  }
}

function fibonacciMaster2(n) {
  let answer = [0,1];
  for ( let i = 2; i <= n; i++) {
    answer.push(answer[i-2]+ answer[i-1]);
  }
  return answer.pop();
}

const fasterFib = fibonacciMaster();

console.log('Slow', fibonacci(35))
console.log('DP', fasterFib(100));
console.log('DP2', fibonacciMaster2(100));
console.log('we did ' + calculations + ' calculations');
```

