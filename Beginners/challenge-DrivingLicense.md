---
layout: default
title: Challenge - Check If the Person Has a Driving License
parent: Rust for Beginners
nav_order: 104
---


# Challenge: Check If the Person Has a Driving License

# Problem Statement 
- A struct Car and Motorbike is provided to you.
- A trait Drive is provided to you which has an abstract method can_drive.

# The task is to
   - implement method `can_drive` for Car
   - implement method `can_drive` for Motorbike
   
# Output 

The output should be `0 ` or `1` based on whether a person can drive or not.

```
1 or 0
```

# Coding Exercise 


```

#![allow(dead_code)] 
//declare a structure
struct Car {
   owner_age:i32,
}
struct Motorbike {
   owner_age:i32,
}
//declare a trait
trait Drive {
   fn can_drive(&self)->i32;
}
//implement the trait
impl Drive for Car{
   fn can_drive(&self)->i32{
      -1
   }
}
impl Drive for Motorbike{
   fn can_drive(&self)->i32{
      -1
   }
}
 


```
Good luck!🤞


   
   
