# Day-3-task

1. 1st Task
   How to compare two different objects without no order
   const _ = require('lodash');
    let obj1 = {
        name : "Person1",
        age : 5
    };
    let obj2 = {
        age : 5,
        name : "Person1"
    };
    console.log(_.isEqual(obj1, obj2))
2. 2nd Task

  const URL = "https://restcountries.com/v3.1/all?fields=name,flags";

const xhr = new XMLHttpRequest();

console.log(xhr)
