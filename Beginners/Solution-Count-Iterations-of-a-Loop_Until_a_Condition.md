---
layout: default
title: Solution 2 - Count Iterations of a Loop Until a Condition
parent: Rust for Beginners
nav_order: 55
---

# Solution 2: Count Iterations of a Loop Until a Condition


# Solution: 

```
fn test(mut x:i32) {
    // define a mutable variable
    let mut count = 0;
    // define a while loop
    while x >= 0 { 
       x = x - 3; // decrement the value of x by 3
       count = count + 1;
    }
    println!("{}", count);
}
fn main(){
    print!("Iterations when x = 21 :");
    test(21);
    print!("Iterations when x = 33 :");
    test(33);
}


```

output;-

```

Iterations when x = 21 :8
Iterations when x = 33 :12

```

# Explanation 

   - On line 3, a mutable variable count is initialized with 0.

   - while construct

      -  while definition
            On line 5,while condition x >= 0 is defined i.e., the loop terminates when x becomes negative.

      - while body

       - The body of while loop is defined from line 5 to line 8.
         -  On line 6, a variable x is decremented by 3.
         -  On line 7, the value of count is incremented each time within the loop.

   - When the loop breaks, the value of count is printed which gives the total number of iterations of the while loop.

