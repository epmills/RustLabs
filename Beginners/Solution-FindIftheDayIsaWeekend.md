---
layout: default
title:  Solution - Find If the Day Is a Weekend
parent: Rust for Beginners
nav_order: 101
---

# Solution - Find If the Day Is a Weekend


Solution: 

```
#![allow(dead_code)]

#[derive(Debug)]

// declare an enum

enum Days{

    Monday, Tuesday, Wednesday, Thursday, Friday, Saturday, Sunday

}

//implement Days methods

impl Days{

    // if the day is a weekend

    fn is_weekend(&self)->i32{

      match self{

        &Days::Saturday=>return 1,

        &Days::Sunday=>return 1,

        _=>return 0

      }

    }

}

fn main() {

    let mut check_day = Days::Saturday;

    println!("Is Saturday a weekend ? : {}", check_day.is_weekend());

    check_day = Days::Monday;

    println!("Is Monday a weekend ? : {}", check_day.is_weekend());

}


```

output 

```
Is Saturday a weekend ? : 1
Is Monday a weekend ? : 0

```

