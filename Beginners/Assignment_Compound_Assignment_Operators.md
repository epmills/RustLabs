---
layout: default
title: Assignment and Compound Assignment Operators
parent: Rust for Beginners
nav_order: 30
---


# Assignment and Compound Assignment Operators

- Assignment Operator 
The assignment operator is used to save a value in the variable.

![](https://raw.githubusercontent.com/sangam14/RustLabs/master/img/assignment-op.png)

# Type 
Rust has only one assignment operator, = . The following table defines the function of the operator.

| operator 	| operation  	| explanation 	| example 	|
|-	|-	|-	|-	|
| operand1 = operand2 	| assign a value  	| assign a value of operand 2  to operand 1 	| a = 1<br>b = a 	|


The following example demonstrates the use of some of the assignment operator in a program:
```
fn main() {
   let a = 2;
   let b = a;
   println!("b = a");
   println!("Value of a:{}", a);
   println!("Value of b:{}", b);
}

```
output:-

```
b = a
Value of a:2
Value of b:2

```
# Compound Assignment Operator 

The compound assignment operator is used to perform an operation and then assign that value to the operand.

![](https://raw.githubusercontent.com/sangam14/RustLabs/master/img/Compound-op.png)

# Types 

The following table summarizes the types of compound assignment operators

| operator 	| operation  	| explanation 	|
|-	|-	|-	|
| operand1 += operand2<br><br>operand1 -= operand2 	| add a value and assign<br><br>subtract a value and assign 	| add left-hand side to right-hand side and then save updated value to left operand<br><br>add right-hand side to right-hand side and then save updated value to left operand   	|
| operand1 /= operand2<br><br>operand1 *= operand2  	| divide a value and assign<br><br>multiple a value and assign 	| divide left-hand side to right-hand side and then save updated value to left operand<br><br>multiply left-hand side to right-hand side and then save updated value to left operand 	|
| operand1 %= operand2 	| modulus and assign 	| take modulus of the left-hand side with right-hand operand and then save updated value to left operand 	|
| operand1 &= operand2 	| Bitwise AND and assign 	| Bitwise AND  of the left-hand side with right-hand operand and then save updated value to left operand 	|
| operand1 \|= operand2 	| Bitwise OR and assign  	| Bitwise OR  of the left-hand side with right-hand operand and then save updated value to left operand 	|
| operand1 ^= operand2 	| Bitwise XOR and assign  	| Bitwise XOR  of the left-hand side with right-hand operand and then save updated value to left operand 	|
| <<= operand1  	| left sift and assign  	| left shift the operand x times then save updated value to operand  	|
| >>= operand1 	| right shift and assign 	| right shift the operand x times then save updated value to operand 	|


The following example demonstrates the use of some of these operators in a program:

```

fn main() {
    //define a mutable variable
    let mut a = 2;
    println!("a:{}", a);
    a += 1;
    println!("a+=1:{}", a);
    println!("a:{}", a);
    a -= 1;
    println!("a-=1:{}", a);
    println!("a:{}", a);
    a /= 1;
    println!("a/=1:{}", a);
    println!("a:{}", a);
    a *= 3;
    println!("a/=3:{}", a);
}



```
output:

```
a:2
a+=1:3
a:3
a-=1:2
a:2
a/=1:2
a:2
a/=3:6

```

# Quiz 

Test your understanding of the assignment and compound assignment operators in Rust.

1. What is the output of the following code?

```
fn main() {
  let mut a = 2;
  let mut b = 3;
  a += a;
  b -= b;
  a *= 1;
  b *= 3;
  a -= 1;
  println!("a: {}", a);
  println!("b: {}", b); 
}


```
A) a: 3 <br> 
   b: 0 <br> 
B) a: 0 <br> 
   b: 3 <br> 
C) a: 2 <br> 
   b: 0 <br> 
D) a: 4 <br> 
   b: 3 <br> 


