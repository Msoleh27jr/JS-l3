![image](https://github.com/user-attachments/assets/f5be54af-9d3e-461d-8d7e-8f4f50874fd2)![js](https://www.tutorialrepublic.com/lib/images/javascript-illustration.png)
# JavaScrict
## 1 **Recursion** <br>
## 2 **CLosure** <br>
<br>
<br>

![Con](https://miro.medium.com/v2/resize:fit:1123/1*jkItJfBy_QzcmwuSanzVuQ.png)
<details>
   <summary>Recursion</summary>

![rec](https://blog.alexdevero.com/wp-content/uploads/2020/11/22-11-20-introduction-to-recursion-in-javascript-how-it-works-and-how-to-use-it-blog.jpg)
## Recursion
  <br>
  
***Recursion in programming is like a
function that keeps calling itself. When a
function does this, its called a
recursively defined function.***

***But there is a rule it has to follow: it must
have a way to stop calling itslef,***

***or it will go on forever. This stopping rule
is called the base case.***

```javascript
function factorial(n) {
    if (n === 0) return 1; // Base case
    return n * factorial(n - 1); // Recursive call
}

console.log(factorial(5)); // Output: 120
```

### And also do not forget about condition becous if you do not put <if> in that's time your code will do your function infinitive

```javascrip

function factorial(n) {
    if (n === 0) return 1;  // <---- ✅
        return n * factorial(n - 1);
    }
}

console.log(factorial(5)); // Output: 120

```
</details>

<br>

![closer](https://media2.dev.to/dynamic/image/width=1280,height=720,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Farticles%2F16uvtgfsbbutez78sr98.png)
<details>
   <summary>Closer</summary>

![closer](https://allma.si/blog/wp-content/uploads/2020/10/what-are-closures.png)
## Loop for
  <br>
  
***Closure is the combination of a function bundled together (enclosed) with references to its
surrounding state (the lexical enviroment). In other words a closure gives you access to an
outer functions scope from an inner function***

***A closure is a function that remembers its outer variables and
can access them. In some languages, this is not possible, or
the function must be written in a special way to create a
closure.***

```javascript
It is righr calling Closer ✅

function counter() {
    let cnt = 0;
    return function() {
        cnt++;
    };
}
let myCounter = counter();
console.log(myCounter);
```

### And also it has anothet way that it is not correct ❌

```javascript

function counter(num1) {
    return function(num2) {
   return num1 + num2
    };
}
console.log(counter(10)(5))
```

</details>
