# Basic programming in JavaScript

We will use Microsoft Visual Studio Code. 

##0 
Before we start we need to install Node. Node is needed for the excercises. 

First step is to install homebrew:

```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

And then install node:

``` 
brew install node

```



## 1
Lets start with this first program:

```
console.log('Hello');
```

or maybe this:

```
console.log(5+4);
```

or

```
console.log('5+4');
```


Questions:

- What do the ' signs do?
- Why is the last sum not calculated?


## 2
To give a value a name, you can use a variable. 

```
let age = 18;

console.log ('You are ' + age);
```

You can use variables for calculations:

```
let age = 18;
let tenYearsAgo = age - 10;

console.log ('You are ' + age);
console.log ('A decade ago ' + tenYearsAgo);
```


Excercise: 

- Can you introduce a second variable that calculates when this is twice the age

Questions:

- What are the rules for naming variables?


## 3
We want to ask the user some questions. This requires a step that is a bit complicated. 
Go to the terminal part in Visual Studio Code. And type in this:

```
npm install readline-sync
```

Now we can create a program:

```
const readlineSync = require('readline-sync');


let age = readlineSync.question('What is your age? ');
console.log ('Your age is: ' + age);

```
From now on you need 


Excercises: 

3. Ask for the user’s name and display it on the screen.
4. Ask for the age of two people and add the ages together.
5. Show the age difference.

Questions:

- Why is there a space after 'What is your age?'


With the function Math.sqrt you can calculate the square root of a number. 

1. Ask for a number and calculate the quare root of that number
2. Honor the Greeks by making a calculator of the Pythagoream theorem: $a^2 + b^2 = c^2$. Ask for a and b, calculate c


## 4
You can use _if_ to check whether a certain condition is there. 


```
const prompt = require('prompt-sync')();

let age = prompt ('What is your age? ');
console.log ('Your age is: ' + age);
if (age >= 18) {
	console.log ('You are an adult');	
}
else {
	console.log ('🐣');
}

```

Questions: 

- What does the >= mean? 
- When is the else executed?


Excercises:

1. Rewrite the *if* so that the first condition handles childeren first
2. Ask for two numbers and display which one is larger.
3. Also show if numbers are equal
4. Ask the user for their age and calculate their maximum heart rate and target heart rate range for exercise. Maximum heart rate: 220 - age. Target heart rate range for exercise: 50% to 85% of the maximum heart rate.

