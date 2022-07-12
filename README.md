# Code Challenge: Higher Order Functions

## Instructions

1. Clone down this assignment to your `code-challenges' directory in AWS Cloud9.  
2. Code your solution using JavaScript in `index.js`. 
3. **Be sure to run and test your code throughly!**
4. By the end of Code Challenge, **commit regularly and push your changes up to Github**.
5. Using the browser, verify that your solution is in your remote repo on Github.

## Code Problems

**All the following problems can be solved using a higher order array method. You cannot use .forEach() to solve the following problems.** 

**Test all your solutions for questions 1-10 with the following variable:** 

`const animals =['cheetah','dog', 'cat', 'dodobird', 'bear', 'dolphin']`

1. Write a function named `pluralize` that takes an array of words that are singular and returns a new array of the same words pluralized.
    
    ```jsx
    pluralize(animals) // ['cheetahs','dogs', 'cats', 'dodobirds', 'bears', 'dolphins']
    ```
    
2. Write a function named `uppercase` that takes an array of strings change every first letter in the string to uppercase.
    
    ```jsx
    uppercase(animals) // ['Cheetah','Dog', 'Cat', 'Dodobird', 'Bear', 'Dolphin']
    ```
    
3. Write a function named `longWords` that takes an array of strings and returns only the strings with more than 3 letters
    
    ```jsx
    longWords(animals) // ['cheetah', 'dodobird', 'bear', 'dolphin']
    ```
    
4. Write a function named `shortWords` that takes an array of strings return the strings with less than 5 letters
    
    ```jsx
    shortWords(animals) // ['dog', 'cat', 'bear']
    ```
    
5. Write a function named `oddLength` that  takes an array of strings and returns an array of just the words that have an odd number of characters:
    
    ```jsx
    oddLength(animals) // ['cheetah','dog', 'cat', 'dolphin']
    ```
    
6. Write a function named `longToShort` that takes an array of strings, and sorts the array by string length in order of greatest to least 
    
    ```jsx
    longToShort(animals) //['cheetah','dog', 'cat', 'dodobird', 'bear', 'dolphin']
    ```
    
    
 8. Write a function named `noVowel` that takes an array of strings and returns an array of strings where all of the vowels have been turned into an x. 
    
    ```jsx
    noVowel(animals) // ['chxxtxh', 'dxg', 'cxt', 'dxdxbxrd', 'bxxr','dxlphxn']
    ```
 9. Write a function named `concatStrings` that takes an array of words and returns a sentence (single string) with all the element strings concatenated together
    
    ```jsx
    concatStrings(animals) // "cheetah dog cat dodobird bear dolphin"
    ```
10. Write a function named `allFour` that takes an array of strings and returns true if all of the strings are a length of 4. 
    
    ```jsx
    allFour(animals) // false
    ```
    
7. Write a function named `sum` that takes an array of numbers and returns the sum of all the numbers in the array.
    
    ```jsx
    const numbers = [22, 15, 1114, 416, 37, 4]
    sum(numbers) // 1608
    ```
    
**Test all your solutions for the questions 1-4 with the following variable:** 

```jsx
const alumni = [
{name:'Jarrit', job:'TPT',language:'JavaScript', age:23}, 
{name:'Stephanie', job:'JPMorgan',language:'JavaScript', age:24}, 
{name:'Devonte', job:'WW',language:'JavaScript', age:23}, 
{name:'Enmanuel', job:'Asana',language:'JavaScript', age:23},
{name:'Shemar', job:'SquareSpace',language:'JavaScript', age:23},
{name:'Cielo', job:'NYT',language:'JavaScript', age:22},
{name:'Carmen', job:'Marcy Lab School',language:'JavaScript', age:21},
{name:'Itzel', job:'Marcy Lab School',language:'JavaScript', age:22},
{name:'Ray', job:'Square Space',language:'JavaScript', age:21},
{name:'Jan', job:'Square Space',language:'JavaScript', age:22},
{name:'Uzma', job:'Thyme Care',language:'JavaScript', age:22}]
```

1. Write a function named `oddJob` that takes an array of objects and returns an array of objects if the job length is an odd number. 
    
    ```jsx
    oddJob(alumni) //returns [
      { name: 'Jarrit', job: 'TPT', language: 'JavaScript', age: 22 },
      { name: 'Enmanuel', job: 'Asana', language: 'JavaScript', age: 21 },
      {
        name: 'Shemar',
        job: 'SquareSpace',
        language: 'JavaScript',
        age: 23
      },
      { name: 'Cielo', job: 'NYT', language: 'JavaScript', age: 21 },
      { name:'Uzma', job:'Thyme Care',language:'JavaScript', age:22 }
    ]
    ```
2. Write a function named `updateLanguage` that takes an array of objects and updates the language value to ES6 if the language is JavaScript, return the entire object. 
    
    ```jsx
    updateLanguage(alumni) // [
      { name: 'Jarrit', job: 'TPT', language: 'ES6', age: 22 },
      { name: 'Stephanie', job: 'JPMorgan', language: 'ES6', age: 21 },
      { name: 'Devonte', job: 'WW', language: 'ES6', age: 23 },
      { name: 'Enmanuel', job: 'Asana', language: 'ES6', age: 21 },
      { name: 'Shemar', job: 'SquareSpace', language: 'ES6', age: 23 },
      { name: 'Cielo', job: 'NYT', language: 'ES6', age: 21 }
    ]
    ```
3. Write a function named `orderedAlumni` that takes an array of objects and sorts the objects by the age of the alumni from oldest to youngest. 
    
    ```jsx
    orderedAlumni(alumni) // returns [
      { name: 'Devonte', job: 'WW', language: 'JavaScript', age: 23 },
      {
        name: 'Shemar',
        job: 'SquareSpace',
        language: 'JavaScript',
        age: 23
      },
      { name: 'Jarrit', job: 'TPT', language: 'JavaScript', age: 22 },
      {
        name: 'Stephanie',
        job: 'JPMorgan',
        language: 'JavaScript',
        age: 21
      },
      { name: 'Enmanuel', job: 'Asana', language: 'JavaScript', age: 21 },
      { name: 'Cielo', job: 'NYT', language: 'JavaScript', age: 21 }
    ]
    ```
4. Write a function named `averageAge` that takes an array of objects and returns the average of all the ages from each age property in each object rounded to the nearest whole number. 
    
    ```jsx
    averageAge(alumni) // 21
    ```
