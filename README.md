# Day-3-task

##1. 1st Task
   How to compare two different objects without no order
   ```
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
```
##2. 2nd Task
```
  const URL = "https://restcountries.com/v3.1/independent?status=true&fields=flags";

const xhr = new XMLHttpRequest();

xhr.open("GET", URL);

xhr.send();


xhr.onreadystatechange = function () {
    
        let countriesData = JSON.parse(xhr.responseText);

        // Loop through the countries and display flags in the console
        countriesData.forEach(country => {
            console.log(`Flag: ${country.flags.svg}`);
        });
    }
```
##3. 3rd Task
   ```
   const URL = "https://restcountries.com/v3.1/all";

const xhr = new XMLHttpRequest();

xhr.open("GET", URL);

xhr.send();


xhr.onreadystatechange = function () {
    
        let countriesData = JSON.parse(xhr.responseText);

        // Loop through the countries and display flags in the console
        countriesData.forEach(country => {
            console.log(`Countries: ${country.name.common},\n 
            Region: ${country.region}\n 
            Sub Region: ${country.subregion}\n
            Population: ${country.population}`
                            );
        });
    }
```
