# Part 2 - Lab 4

## Question 1

1. 3

Line 12 prints the value of i, which is defined in the for loop. And since the for loop loops through the given array, which is a length of 3, line 12 prints 3.

## Question 2

2. 150

Line 13 prints the value of discountedPrice, which is defined in the for loop. The for loop loops through the elements in the given array, and then multiplies it by discount parameter. discountedPrice then stores the current value in the for loop. This means that at the end of the for loop, it will print the last element, which is 300, multiplied by the discount, which is 0.5. The value of discountedPrice is 150, so at line 13, it will print 150.

## Question 3

3. 150

Line 14 prints the value of finalPrice, which is defined in the for loop. The for loop loops through the elements in the given array, fineds the discoundedPrice, then rounds it. discountedPrice then stores the current value in the for loop. This means that at the end of the for loop, it will store  the last element, which is 300, multiplied by the discount, which is 0.5. The value of discountedPrice is 150, and that rounded will still be 150, so at line 14, it will print 150.

## Question 4

1. [ 50, 100, 150 ]

This function returns the value of discounted. discounted is an empty array variable, and in the funciton we continuously push the finalPrice value in the array. So the funciton will return an array of all the finalPrice values of all the elements of the given parameter.

## Question 5

5. ERROR

The reason that there is an error is because i is defined with 'let' in the for loop block, so the code isn't able to print the i variable since line 12 is outside the for loop.

## Question 6

6. ERROR

The reason that there is an error is because discountedPrice is defined with 'let' in the for loop block, so the code isn't able to print the discountedPrice variable since line 13 is outside the for loop.

## Question 7

7. 150

Since finalPrice was defined with 'let' **outside** the for loop, the current block is the entire inside of the function. This allows the code in line 14 to print out the value of finalPrice.

## Question 8

8. [ 50, 100, 150 ]

This function returns the value of discounted. discounted is an empty array variable, and in the funciton we continuously push the finalPrice value in the array. So the funciton will return an array of all the finalPrice values of all the elements of the given parameter. There is no error since we aren't trying to call a variable from outside it's block.

## Question 9

9. ERROR

Like question 5, the reason that there is an error is because i is defined with 'let' in the for loop block, so the code isn't able to print the i variable since line 11 is outside the for loop.

## Question 10

10. 3

Line 12 prints the length of prices, which is the input parameter array. In this case, the array is of size 3, so it prints 3 in line 12.

## Question 11

11. [ 50, 100, 150 ]

Similar to the original function, it returns the value of discounted, which is an array consisting of all the discounted prices (in this case without rounding, but they are still the same values).

## Question 12

12. Part:

    A. **student.name**
    B. **student['Grad Year']**
    C. **student.greeting()**
    D. **student[Favorite Teacher'].name**
    E. **student.courseLoad[0]**

## Question 13

13. Part:

    A. '3' + 2 = **'32'**

    In JavaScript, + can be used for adding and concatinating strings. In this case, '3' and 2 were concatinated to make a string of '32'.

    B. '3' - 2 = **1**
    
    In JavaScript, - can only be used for subtraction, so string '3' turned into an integer, and outputed 3 - 2, which is 1.

    C. 3 + null = **3**

    In this case, null is converted into a 0, which makes the equation 3 + 0, which is 3.

    D. '3' + null = **'3null'**

    In this case, null is converted into a string 'null', and since + can concatinate, it concatinated '3' and 'null' to be '3null'.

    E. true + 3 = **4**

    In this case, true, which maps to 1, turns to a 1. The equation turns to 1 + 3, which is 4.

    F. false + null = **0**

    In this case, false, which maps to 0, turns to a 0. null is also turned into a 0. The equation turns to 0 + 0, which is 0.

    G. '3' + undefined = **'3undefined'**
    
    In this case, undefined is converted into a string 'undefined', and since + can concatinate, it concatinated '3' and 'undefined' to be '3undefined'.

    H. '3' - undefined = **3**

    In this case, '3' is converted to an interger and undefined is converted into a NaN, it's interger format. And since any arithmetic with NaN equals to NaN, the equation is 3 + NaN, which is still NaN.

## Question 14

14. Part:

    A. '2' > 1 = **true**

    '2' is converted to an integer, so the expression is 2 > 1, which is true.

    B. '2' < '12' = **false**
    
    Since the expression is of strings, it is compared in a lexicorgraphic style, or dictionary style, where it sees which element in a string comes first. In this case, 2 comes after 1, so it is false.

    C. 2 == '2' = **true**

    Since == allows for the variables to change types before comparing, '2' becomes an integer, so the expression is 2 == 2, which is true.

    D. 2 === '2' = **false**

    === doesn't allow for variables to change types. Since 2 is strictly not equal to '2', it outputs false.

    E. true == 2 = **false**

    In this case, true changes into a integer 1, and since 1 is not equal to 2, it outputs false.

    F. true == Boolean(2) = **true**

    The Boolean funciton converts its parameters into a boolean value, so 2 becomes true, and since true equals to true, it outputs true.

## Question 15

15. '==' allows what called type coercion, which basically means that the variables are allowed to change types before comparing if they are equal
    '===' doesn't allow type coercion. It strictly compares if the two values are exactly equal.

## Question 16

16.   In [part2-question16.js](part2-question16.js)
      Code:
      ```
        for (const key in statistics) {
            if (key[0] === 'r' || statistics[key] % 2 == 1) {
                console.log(statistics[key]);

            }
        }
      ```

## Question 17

17. [ 2, 4, 6 ]
    
We call modifyArray([1, 2, 3], doSomething); I then look to see at what modifyArray() does. Then I see that it makes a new array and pushes the old elements into the new array after the elements are modified by callback. In this case, callback is a function doSomething() that basically doubles the inputed number. That means all the orginal elements from the original array will be doubled.

## Question 18

18.   In [part2-question18.js](part2-question18.js)
      Code:
      ```
        function timeEverySecond() {
            let d = new Date();
            let time = d.toLocaleTimeString();
            console.log(time);
        }

        setInterval(timeEverySecond, 1000);
      ```

## Question 17

17. Output:
1
4
3
2
    
It instantaneously prints 1, 4, and 3. But a second after the program runs, it prints 2.