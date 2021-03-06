---
layout: default
title: Solution 3 - Find nth Fibonacci Number
parent: Rust for Beginners
nav_order: 70
---

# Solution 3 - Find nth Fibonacci Number

```
fn fibonacci(term: i32) -> i32 {
    match term {
        0 =>  0,
        1 =>  1,
        _ => fibonacci(term-1) + fibonacci(term-2),
    }
}
fn main(){
    println!("fibonacci(4)={}",fibonacci(4));
}



```

output 

```
fibonacci(4)=3

```
# Explanation 

A recursive function, fibonacci, takes a parameter term of type i32 and returns an integer of type i32, i.e., the nth term of the Fibonacci number.

The recursive function has two parts: the base case, and the recursive case.
  - base case
      -  match takes the term and if it matches with 0 it returns 0 and if it matches with 1 it returns 1
  - recursive case
      -  It decrements the value of the term by 1. A recursive call is made with argument term - 1 or term - 2 and that the function execution can’t proceed until the recursive calls return. Now the answer before the + operator is calculated.
      -  It then decrements the value of the term by 2. A recursive call is made with argument term - 1 or term - 2 and that the function execution can’t proceed until the recursive calls return. Now the answer after the + operator is calculated.
      -  It simply adds the two values and returns the result.
      
      
      


