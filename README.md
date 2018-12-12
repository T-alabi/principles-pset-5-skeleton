# Problem Set 5

Problem Set 5 challenges your ability to use conditional and iterative control structures to implement more complicated algorithms. Like the previous problem set, you should be diplaying your solutions in the `output` boxes. You can compare your solutions against mine in the `result` boxes. With exception of adding the `onclick` attributes, you shouldn't modify the HTML file.

## Getting Started

To get started, you'll need to create a [GitHub](https://github.com/) repository to store your Problem Set 5 code. After cloning my skeleton repository, you'll need to setup a remote to push your code to your repository instead of mine. Steps to accomplish this are outlined below.

### Setup

01. Login to your [GitHub](https://github.com/) account and create a new repository named `problem-set-5`.
02. In GitBash, navigate to your `APCSP` folder.
03. Clone my skeleton repository from [GitHub](https://github.com/). This will make a copy of my repository and store it locally.
```
git clone git@github.com:rwilson-ucvts/principles-pset-5-skeleton.git
```
04. The cloning process will have created a folder named `principles-pset-5-skeleton`. Rename this folder to `pset4`.
```
mv principles-pset-5-skeleton pset5
```
05. Change directories to get into your `pset5` folder.
```
cd pset5
```
06. Originally, the remote will be pointing at my repository. We need to overwrite this.
```
git remote rename origin upstream
```
07. Lastly, we need to add a new remote that points at the repository you created earlier. Make sure you replace `YOUR-USERNAME` with your actual username.
```
git remote add origin git@github.com:YOUR-USERNAME/problem-set-5.git
```
08. Launch Atom and select `File > Add Project Folder...`.
09. Navigate to your `pset5` directory and click `Open`.

## Exercises

Problem Set 5 contains 7 exercises, each of which will be written in separate functions. There are several segments of code that should not be modified. They will help you to implement and test your solutions.

### Exercise 1 (`Mario.`)

Write a function that prompts the user for a height, and prints a Mario-style half-pyramid of that height.
```
     ##
    ###
   ####
  #####
 ######
 ```
Height values must be integers within the range [1, 23]. Users should be continuously re-prompted until they comply with this restriction.

As always, certain portions of the starter code are critical to the the feedback script. Please do not modify these sections. They are clearly marked.

All output should be displayed on the page, not printed to the console.

### Exercise 2 (`Mario, Again.`)

Write a function that prompts the user for a height, and prints a Mario-style pyramid of that height.
```
    ##  ##
   ###  ###
  ####  ####
 #####  #####
######  ######
```
Height values must be integers within the range [1, 23]. Users should be continuously re-prompted until they comply with this restriction.

As always, certain portions of the starter code are critical to the the feedback script. Please do not modify these sections. They are clearly marked.

All output should be displayed on the page, not printed to the console.

### Exercise 3 (`Credit.`)

Write a function that prompts the user for a credit card number (valid and invalid examples will be provided), and displays either:
* an invalid image (provided)
* an American Express image (provided)
* a Mastercard image (provided)
* a Visa image (provided)

We'll use Luhn's algorithm to determine the validity of a credit card number. Review the steps of the algorithm below.

* Multiply every other digit by 2, starting with the number’s second-to-last digit, and then add those products' digits together.
* Add the sum to the sum of the digits that weren’t multiplied by 2.
* If the total’s last digit is 0 (or, put more formally, if the total modulo 10 is congruent to 0), the number is valid!

American Express uses 15-digit numbers, starting with 34 or 37. Mastercard uses uses 16-digit numbers, starting with 51, 52, 53, 54,
or 55. Visa uses 13- or 16-digit numbers, starting with 4. Examples are shown below.

* 378282246310005 should verify as American Express.
* 371449635398431 should verify as American Express.
* 5555555555554444 should verify as Mastercard.
* 5105105105105100 should verify as Mastercard.
* 4111111111111111 should verify as Visa.
* 4012888888881881 should verify as Visa.

Credit card numbers must be integers. Users should be continuously re-prompted until they comply with this restriction.

As always, certain portions of the starter code are critical to the the feedback script. Please do not modify these sections. They are clearly marked.

All output should be displayed on the page, not printed to the console.

### Exercise 4 (`Guess.`)

Write a function that generates a random number, and asks the user to try to guess this number. When all is said and done, your function should output the random number and the number of attempts it took the user to correctly guess that number. Your function should also provided helpful hints, indicating whether the most recent guess was greater than or less than the target.

Random numbers must be between 1 and 1000. User guesses must be integers within the range [1, 1000], and users should be continuously re-prompted until they comply with this restriction. In the event a user guesses something that violates this restriction, an attempt should not be recorded.

As always, certain portions of the starter code are critical to the the feedback script. Please do not modify these sections. They are clearly marked.

All output should be displayed on the page, not printed to the console.

### Exercise 5 (`Hurricane.`)

Write a function that prompts the user to enter a windspeed, and prints the hurricane category (if applicable) for that windspeed. We'll be using the Saffir-Simpson scale, shown below in MPH.

* Category 5: 157+
* Category 4: 130-156
* Category 3: 111-129
* Catgeory 2: 96-110
* Category 1: 74-95
* Tropical Storm: 39-73

Windspeeds must be non-negative integers in the range (-Infinity, Infinity), and users should be continuously re-prompted until they comply with this restriction.

As always, certain portions of the starter code are critical to the the feedback script. Please do not modify these sections. They are clearly marked.

All output should be displayed on the page, not printed to the console.

### Exercise 6 (`Gymnastics.`)

Write a function that prompts the user to enter six scores. From those six scores, the lowest and highest should be discarded. An average score should be computed from the remaining four. Your function should output the discarded scores, as well as the average score.

Scores must be real numbers in the range [0.0, 10.0], and users should be continuously re-prompted until they comply with this restriction.

As always, certain portions of the starter code are critical to the the feedback script. Please do not modify these sections. They are clearly marked.

All output should be displayed on the page, not printed to the console.

### Exercise 7 (`Report Card.`)

Write a function that prompts the user to enter test, quiz, and homework grades for the marking period. Users can enter as many grades of each category, entering -1 to signal they are finished. Your function should output the user's final grade, where tests, quizzes, and homework are weighted at 60%, 30%, and 10%, respectively.

Grades must be real numbers in the range [0.0, 100.0], and users should be continuously re-prompted until they comply with this restriction. The only exception is -1, which signals the user is finished entering grades for that category.

As always, certain portions of the starter code are critical to the the feedback script. Please do not modify these sections. They are clearly marked.

All output should be displayed on the page, not printed to the console.

## Deadline

Your Canvas submission is due at or before 11:59pm on Monday, December 3, 2018.

### Submission Requirements

All that is required for submission is the public URL to your [GitHub](https://github.com/) repository for this problem set. If you forgot how to create a public URL for your repository, reread the [original instructions from Problem Set 3¾](https://canvas.instructure.com/courses/1408038/pages/github-pages?module_item_id=19614011).
