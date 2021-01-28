# Part 1
## Variables & Scoping
1. It prints the length of prices because var has no block scope (visible through "for" and not local)  
2. prints discounted price  
3. prints finalPrice  
4. It returns [50, 100, 150].  It correctly iterates through the for loop and prints the discounted prices through the given calculation  
  
5. referenceError because i is a local variable of the for loop.  
6. referenceError because discountedPrice is a local variable of the for loop.  
7. It should be able to return the finalPrice assuming the rest of the variables are declared properly.  This is because it is declared before the loop.  
8. Assuming it is able to return it will return `[50, 100, 150]`.  As it is, it will not reach the return due to referenceErrors.

9. Should have referenceError because i is a local variable of the for loop (let supports this)  
10. There should be another referenceError because discountedPrice is a local variable inside the code block.  
11. finalPrice has an error because it is reassigned in the loop. However, if we removed these errors, it should log 0 as it is a constant which should remain unchanged.    
12. discounted once again should have an error during the loop (const reassignment), so we are not expecting a return.  If anything were to return, the array could be non-empty as the constant is simply setting the reference to the array. We can still push to it, but this is bad programming.  If we did push, the values would be `[50, 100, 150]`.  
  
## Data Types  
13.  A. student.name  
     B. student.["Grad Year"]  
     C. student.greeting  
     D. student.["Favorite Teacher"].name
     E. student.courseLoad[1] (index = 1?? or 0 if you're talking about the initial index)

## Basic Operators & Type Conversion
14. Arithmetic
    A. 32.  '3' is a string literal so it appends 2 onto the string and returns the string 32. (the '+' functions as append here)  
    B. 1.  Since '-' is not a function for strings, JS converts 3 into a number and attempts to subtract. This returns 1.
    C. 3.  null represents the absence of value.  In this case it is equal to 0 and thus we get 3.  
    D. 3null. null is turned into its string representation and appended  
    E. 4.  Since we are adding, JS converts true to 1.  
    F. 0.  false is converted to its numeric value because the operation is addition (and boolean addition causes it to be converted ex. true + true = 2), 0, and null is added to it resulting in 0.
    G. 3undefined.  This is appending undefined to the string literal 3.  
    H. NaN. Returns undefined because we are attempting to subtract undefined from 3.  (undefined is different from null, it represents NaN and 3 - NaN results in an undefined value)  
15. Comparison  
    A. true. 2 becomes a number.  
    B. false.  They are now both strings.  2 is not less than 1, so we get false.
    C. true.  They are equal with type conversion.
    D. false. They are not strictly equal. (No type conversion)  
    E. false. true == 1  
    F. true.  Any value other than 0, empty string, null, etc is considered to be true when converted thus we get true === true which returns true.  

16.  == includes type conversion, === does not and is strict equality.

## Conditionals
17. `How are you?`  This prints because the first condition 2 == true is false as shown in 15.  however Boolean(2) === true and this statement prints.  
## Loops  
18. in part1-question18.js  
  
## Functions
19. `[6,8,10]`  What this function is doing is calling doSomething with the number in the array and then another function that will function as the callBack parameter in doSomething.  Each doSomething first adds 2 to `array[i]` and then calls the callback parameter of doSomething which multiplies it by two.  This results in (1 + 2) * 2 = 6, (2 + 2)*2 = 8, (3 + 2) * 2 = 10.  Each of these were pushed into newArr which is returned, resulting in this answer.  

## setInterval(), setTimeout(), clearTimeout()  
20.  TODO: in part1-question20.js
21.  
```javascript 
1
4
3
2
```
This is the case in node as 3 is executed in the next event cycle which comes after 4 is logged.  (Must complete thread where setTimeout function is called, which means that it finishes running code down to console.log(4) and then immediately calls the 2nd setTimeout)

