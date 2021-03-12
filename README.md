# m1d5

/*
    ASSIGNMENT RULES
    - All the answers must be written in JavaScript
    - The solution must be pushed to the repository and be available for the tutors by the end of the day
    - You can ask for help, reach the Teaching Assistants if needed
    - You can google / use StackOverflow BUT we suggest you to use just the material provided
    - You can test your code in a separate file or de-commenting the single exercises in this one.
      You can use the bash terminal, the VSCode terminal or the one embedded in your Operating System if you're using macOS or Linux.
    - Complete as many exercise that you can
    - Publish them into your own GitHub account and upload repository link on Eduflow before 16.30 (Berlin Time) 
*/

//JS Basics

/* Ex.A
   Create a variable called "test" and assign a string to it.
*/
console.log("------------------------------ EXERCISE A -----");

let test = "This is a string for the variable test";
console.log("test");

console.log("\n");

/* Ex.B
    Create a variable called "sum" and assign to it the result of the sum between 10 and 20.
*/
console.log("------------------------------ EXERCISE B -----");

let sum = 10 + 20;
console.log("sum");

console.log("\n");

/* Ex.C 
    Create a variable called "random" and assign to it a random number between 0 and 20 
    (it should be randomly created at each execution).*/
console.log("------------------------------ EXERCISE C -----");

const generateRandomNumber = function (min, max) {
  let random = Math.floor(Math.random() * (max - min) + min);
  return random;
  /* I used the Math.random() to generate random numbers between 0 (inclusive) and 1 (exclusive). 
  Then, by using the Math.floor() function, I generate larger the numbers. */
};
console.log(generateRandomNumber(0, 20));
console.log(generateRandomNumber(0, 20));
console.log(generateRandomNumber(0, 20));

let random = console.log("\n");
/* Ex.D
    Create a variable called "me" and assign to it an object containing the following information: 
    name = your name, surname = your surname, age = your age.
*/
console.log("------------------------------ EXERCISE D -----");

const me = {
  nam: "Ingrid",
  surname: "Oncken",
  age: 34,
};
console.log(me);
console.log("\n");
/* Ex.E 
    Programmatically remove the age property from the previously create object.
*/
console.log("------------------------------ EXERCISE E -----");

console.log(me);
delete me.age;
console.log(me);

console.log("\n");
/* Ex.F 
   Programmatically add to the object me an array called "skills", containing the programming languages you 
   know right now.
*/
console.log("------------------------------ EXERCISE F -----");

console.log(me);
me.skills = ["Java", "Javascript"];
console.log(me);

console.log("\n");
/* Ex.G 
   Programmatically remove the last skill from the "skills" array inside the "me" object.
*/
console.log("------------------------------ EXERCISE G -----");

console.log("\n");
// JS Functions
/* Ex.1
    Write a function called "dice"; it should randomize an integer number between 1 and 6.
*/
console.log("-------------------- EXERCISE 1 -----");

const dice = function (min, max) {
  let random16 = Math.floor(Math.random() * (max - min) + min);
  return random16;
};
console.log(dice(1, 6));
console.log(dice(1, 6));
console.log(dice(1, 6));
console.log(dice(1, 6));

console.log("\n");
/* Ex.2 
    Write a function called "whoIsBigger" which receives 2 numbers as parameters and returns the biggest one.
*/
console.log("-------------------- EXERCISE 2 -----");

const whoIsBigger = function (n1, n2) {
  let intN1 = parseInt(n1);
  let intN2 = parseInt(n2);
  let subN1N2 = intN1 - intN2;

  if (subN1N2 < 0) {
    console.log(`Number ${intN2} is bigger than ${intN1}`);
  } else if (subN1N2 > 0) {
    console.log(`Number ${intN1} is bigger than ${intN2}`);
  } else {
    console.log(`They're the same number!`);
  }
};
whoIsBigger(3, 2);
whoIsBigger(5, 5);
whoIsBigger(9, 7);

console.log("\n");
/* Ex.3
    Write a function called "splitMe" which receives a string as a parameter and returns an array with every word 
    in that string. Ex. splitMe("I love coding") => returns ["I", "Love", "Coding"]
*/
console.log("-------------------- EXERCISE 3 -----");

// I DON'T KNOW HOW TO MAKE A FUNCTION OF IT AND RETURN THE ARRAY 😟
splitMe = "I love coding"; // HOW THIS WORKS IF splitMe HAS NOT BEEN DECLARED???
let mySplit = splitMe.split(" ");
console.log(mySplit);

console.log("\n");

/* Ex.4
    Write a function called "deleteOne" which receives a string and a boolean as parameters. 
    If the boolean value is true it should return the string without the first letter, 
    otherwise it should remove the last one from it.
*/
console.log("-------------------- EXERCISE 4 -----");

const deleteOne = function (str4Delete, bool) {
  if (bool === true) {
    // I HAVE NO IDEA HOW TO COMPARE THE STRING BOOL WITH THE BOOLEAN VALUE
    let remove1st = str4Delete.substring(1);
    return remove1st;
  } else {
    return str4Delete;
  }
};
deleteOne();
console.log(`Happy`, true);

console.log("\n");
/* Ex.5
   Write a function called "onlyLetters" which receives a string as a parameter and returns it removing all the digits.
   Ex.: onlyLetters("I have 4 dogs")  => returns "I have  dogs"
*/
console.log("-------------------- EXERCISE 5 -----");

const onlyLetters = function (lettersNumbers) {
  let removeNum = lettersNumbers.replace(/[0-9])/g, " ");
  return removeNum;
};
onlyLetters("I have 4 dogs");
console.log(onlyLetters);

//var withNoDigits = questionText.replace(/[0-9]/g, ""); ===> EXTRACTED FROM THE INTERNET

console.log("\n");
/* Ex.6 
   Write a function called "isThisAnEmail" which receives a string as a parameter and returns true if the string is a valid email address.
*/
console.log("-------------------- EXERCISE 6 -----");



console.log("\n");
/* Ex.7
   Write a function called "whatDayIsIt" that should return the current day of the week.
*/

/* Ex.8
    Write a function called "rollTheDices" which receives a number as a parameter.
    It should invoke the dice() function defined in Ex1 the specified amount of times,
    and return an object containing a "sum" property holding the sum of all values extracted
    and a "values" array containing the single values of the dicerolls themselves.
    Example: RollTheDices(3) => returns {
        sum: 10
        values: [3, 3, 4]
    }
*/

/* Ex.9
   Write a function called "howManyDays" which receives a date as a parameter and should return the number of days passed since that date.
*/

/* Ex.10
   Write a function called "isTodayMyBirthday" which should return true if today's your birthday, false otherwise.
*/

// JS Arrays // Objs
// NOTE: movies array is defined at the end of this file!

/* Ex.11
   Write a function called "deleteProp" which receives an object and a string as parameters, and returns the given object after deleting its property named as the given string.
*/

/* Ex.12 
    Write a function called "olderMovie" which finds the oldest movie in the array provided at the end of this file.
*/

/* Ex.13
    Write a function called "countMovies" which returns the number of movies contained in the array provided at the end of this file.
*/

/* Ex.14
    Write a function called "onlyTheTitles" which creates an array with just the titles of the movies provided in the array at the end of the file.
*/

/* Ex.15
   Write a function called "onlyInThisMillennium" which returns only the movies produced in this millennium.
*/

/* Ex.16 
    Write a function called "getMovieById" which receives an id as a parameter and returns the movie with the given id.
*/

/* Ex.17
    Write a function called "sumAllTheYears" which returns the sum of all the years in which the movies provided have been produced.
*/

/* Ex.18
    Write a function called "searchByTitle" which receives a string as a parameter and returns all the movies which contain that string in the title.
*/

/* Ex.19
    Write a function called "searchAndDivide" which receives a string as a parameter and returns an object;
    this object should contain an array called "match", made by all the movies which contain the given string in the title,
    and another array "unmatch" with all the remaining ones.
*/

/* Ex.20
   Write a function called "removeIndex" which receives a number as a parameter and returns the movies array without the element in the given position.
*/

// [EXTRAS] JS Advanced

/* Ex.21
  Create a function called "halfTree" which receives a number as a parameter and builds an "*" half tree with the given height.
  Example:
  halfTree(3)
  *
  **
  ***
*/

/* Ex.22 
  Create a function called "tree" which receives a number as a parameter and builds an "*" tree with the given height.
  Example: 
  tree(3)
    *  
   *** 
  *****
*/

/* Ex.23
  Create a function called "isItPrime" that receives a number as a parameter and returns true if the given number is a prime number.
*/

/* This movies array is used throughout the exercises. Please don't change it :)  */
const movies = [
  {
    Title: "The Lord of the Rings: The Fellowship of the Ring",
    Year: "2001",
    imdbID: "tt0120737",
    Type: "movie",
    Poster:
      "https://m.media-amazon.com/images/M/MV5BN2EyZjM3NzUtNWUzMi00MTgxLWI0NTctMzY4M2VlOTdjZWRiXkEyXkFqcGdeQXVyNDUzOTQ5MjY@._V1_SX300.jpg",
  },
  {
    Title: "The Lord of the Rings: The Return of the King",
    Year: "2003",
    imdbID: "tt0167260",
    Type: "movie",
    Poster:
      "https://m.media-amazon.com/images/M/MV5BNzA5ZDNlZWMtM2NhNS00NDJjLTk4NDItYTRmY2EwMWZlMTY3XkEyXkFqcGdeQXVyNzkwMjQ5NzM@._V1_SX300.jpg",
  },
  {
    Title: "The Lord of the Rings: The Two Towers",
    Year: "2002",
    imdbID: "tt0167261",
    Type: "movie",
    Poster:
      "https://m.media-amazon.com/images/M/MV5BNGE5MzIyNTAtNWFlMC00NDA2LWJiMjItMjc4Yjg1OWM5NzhhXkEyXkFqcGdeQXVyNzkwMjQ5NzM@._V1_SX300.jpg",
  },
  {
    Title: "Lord of War",
    Year: "2005",
    imdbID: "tt0399295",
    Type: "movie",
    Poster:
      "https://m.media-amazon.com/images/M/MV5BMTYzZWE3MDAtZjZkMi00MzhlLTlhZDUtNmI2Zjg3OWVlZWI0XkEyXkFqcGdeQXVyNDk3NzU2MTQ@._V1_SX300.jpg",
  },
  {
    Title: "Lords of Dogtown",
    Year: "2005",
    imdbID: "tt0355702",
    Type: "movie",
    Poster:
      "https://m.media-amazon.com/images/M/MV5BNDBhNGJlOTAtM2ExNi00NmEzLWFmZTQtYTZhYTRlNjJjODhmXkEyXkFqcGdeQXVyNDk3NzU2MTQ@._V1_SX300.jpg",
  },
  {
    Title: "The Lord of the Rings",
    Year: "1978",
    imdbID: "tt0077869",
    Type: "movie",
    Poster:
      "https://m.media-amazon.com/images/M/MV5BOGMyNWJhZmYtNGQxYi00Y2ZjLWJmNjktNTgzZWJjOTg4YjM3L2ltYWdlXkEyXkFqcGdeQXVyNTAyODkwOQ@@._V1_SX300.jpg",
  },
  {
    Title: "Lord of the Flies",
    Year: "1990",
    imdbID: "tt0100054",
    Type: "movie",
    Poster:
      "https://m.media-amazon.com/images/M/MV5BOTI2NTQyODk0M15BMl5BanBnXkFtZTcwNTQ3NDk0NA@@._V1_SX300.jpg",
  },
  {
    Title: "The Lords of Salem",
    Year: "2012",
    imdbID: "tt1731697",
    Type: "movie",
    Poster:
      "https://m.media-amazon.com/images/M/MV5BMjA2NTc5Njc4MV5BMl5BanBnXkFtZTcwNTYzMTcwOQ@@._V1_SX300.jpg",
  },
  {
    Title: "Greystoke: The Legend of Tarzan, Lord of the Apes",
    Year: "1984",
    imdbID: "tt0087365",
    Type: "movie",
    Poster:
      "https://m.media-amazon.com/images/M/MV5BMTM5MzcwOTg4MF5BMl5BanBnXkFtZTgwOTQwMzQxMDE@._V1_SX300.jpg",
  },
  {
    Title: "Lord of the Flies",
    Year: "1963",
    imdbID: "tt0057261",
    Type: "movie",
    Poster:
      "https://m.media-amazon.com/images/M/MV5BOGEwYTlhMTgtODBlNC00ZjgzLTk1ZmEtNmNkMTEwYTZiM2Y0XkEyXkFqcGdeQXVyMzU4Nzk4MDI@._V1_SX300.jpg",
  },
  {
    Title: "The Avengers",
    Year: "2012",
    imdbID: "tt0848228",
    Type: "movie",
    Poster:
      "https://m.media-amazon.com/images/M/MV5BNDYxNjQyMjAtNTdiOS00NGYwLWFmNTAtNThmYjU5ZGI2YTI1XkEyXkFqcGdeQXVyMTMxODk2OTU@._V1_SX300.jpg",
  },
  {
    Title: "Avengers: Infinity War",
    Year: "2018",
    imdbID: "tt4154756",
    Type: "movie",
    Poster:
      "https://m.media-amazon.com/images/M/MV5BMjMxNjY2MDU1OV5BMl5BanBnXkFtZTgwNzY1MTUwNTM@._V1_SX300.jpg",
  },
  {
    Title: "Avengers: Age of Ultron",
    Year: "2015",
    imdbID: "tt2395427",
    Type: "movie",
    Poster:
      "https://m.media-amazon.com/images/M/MV5BMTM4OGJmNWMtOTM4Ni00NTE3LTg3MDItZmQxYjc4N2JhNmUxXkEyXkFqcGdeQXVyNTgzMDMzMTg@._V1_SX300.jpg",
  },
  {
    Title: "Avengers: Endgame",
    Year: "2019",
    imdbID: "tt4154796",
    Type: "movie",
    Poster:
      "https://m.media-amazon.com/images/M/MV5BMTc5MDE2ODcwNV5BMl5BanBnXkFtZTgwMzI2NzQ2NzM@._V1_SX300.jpg",
  },
];
