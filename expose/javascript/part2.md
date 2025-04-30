1. ^^^ What will happen at line 12 and why? If the code causes an error, explain why. ^^^
    line 12 will return 3 because all of the created variables are stated as var meining its values can be accesed outside of its blocks, so even though the for loop has ended the variable i is still accsessable. 

2.  ^^^ What will happen at line 13 and why? If the code causes an error, explain why. ^^^
    line 13 returns the value 150, this is because discoundedPrice holds the last compiuted value which is 150(300 * (1 - 0.5) 

3. ^^^ What will happen at line 14 and why? If the code causes an error, explain why. ^^^
   Simular to line 13 the value 150 is returned too, this is bacause finalPrice holds on to the last iteration variable too. 

4. ^^^ What will this function return? Give a brief explanation why. If the code causes an error, explain why. ^^^
    This function returns the list of prices with their new discount so for this example, discountPrices([100, 200, 300], 0.5) returns [50, 100, 200]. This can be shown thouh the lines "discountedPrice = prices[i] * (1 - discount);" and "finalPrice = Math.round(discountedPrice * 100) / 100;" which first provides the discounted price by multiplying it by the discount then final price turns that value into a whole number 

5. ^^^ What will happen at line 12 and why?  If the code causes an error, explain why. ^^^ (assume this function is being called like the others: discountPrices([100, 200, 300], 0.5)).
    This line will produce a RefernceError because the variable i is declared within the for loop block and since line 12 tries to accsess it outside of this block an error is given. This is because of let's properties that keeps its value with its block



6. ^^^ What will happen at line 13 and why? If the code causes an error, explain why. ^^^
    Simular to line 12 discountdPrice is defined within the for loop block so it will not be accsessable outisde of it. 

7. ^^^ What will happen at line 14 and why? If the code causes an error, explain why. ^^^
    The Value 150 is returned, this is because the variable final price is created within the same block as line 14 so its value can be accsessed. even though it is eddited within the for loop its value is still held because of its still within the block it was created. 

8. ^^^ What will this function return? Give a brief explanation. If the code causes an error, explain why. ^^^
    Sumular to question 4 this code will also return [50, 100, 150]. Since lines 12 and 13 are commented out this code will never try and accsess let variables outside of their block so it can perform its function correctly. 

9. ^^^ What will happen at line 11 and why? If the code causes an error, explain why. ^^^
    This will return a ReferenceError: this is because simular to the previous function i is defined within the for loop block so it can not be accsesed outisde of it. 

10. line 12 returns the value 3. This is because the value was declared at the begining of the function which is within the same block as line 12 so there is no problem with refrence, then since length is never eddited thoughout the function there is no problems with a TypeError. 

11. This function will return 3 coppies of the function itself [discountedPrices, discountedPrices discountedPrices]. this is because you compute discounted price in each loop, then it ends up pushing the function discountPrices rather than the number value.
    
12. Given the above Object, write the notation for:  (These should be in your part2.md)
Accessing the value of the name property in the student object
A. 
    student.name
B.
    student['Grad Year']
C.
    student.greeting()
D.
    student['Favorite Teacher'].name
E.
    student.courseLoad[0]

13. Arithmetic
A.
    '32'   // + with a string causes string concatenation
B.
    1     // '-' forces artimetic conversion so it becomes (3 -2 = 1)
C.
    3     // null is readed as 0 in aritmetic operations (3+ 0 = 3)
D.
    3null // +  causes string concatnation even will null
E.
    4     // true is treated as 1 in aretmetic so its (1 + 3 = 4)
F.
    0     // false is treated as 0 and so is null so its just (0 + 0 = 0)
G.
    3undefined // + causes a string concatenation even with undefiend
H.
    NaN   // the - operator tried to convert both into numbers which is ok for 3 but undefined cannot be convered into a number so you just get NaN

14.  Comparison
A.
    true, Js uses type coercion so the '2' is just converted into the integer value 2 (2 > 1 ; true)
B.
    false, when both values are strings instead of type coercion it treats it lexicographicly and since 2 comes after 1 in unicode ('2' < '12'; false)
C.
    true, the == allows for type coercion too so the '2' becomes 2 just like problem A
D. 
    false, === means strict equality comparison so there is no type coercion meaning they are not equal.
E.  
    false, true becomes 1 just like in Arithmetic operations, so it becomes (1 == 2; false) 
F.  
    true, in a Boolean context 2 is a truthy value so both sides equate to true

15.  Explain the difference between the == and === operators.
    == stands for a loose equaluty, this means that as long as the values are the same after converting types then it will be true. where as === stands for a strict equality so it only cares about what the 2 values are and will check to make sure the types are the same too. This means that '2' == 2 can be true but '2' === 2 would be false, as no coercion was made. 

16. Given the above Object, write a for...in loop that will iterate through it and print out the value of the property if the property starts with the letter r, or if the value of that property is an odd number.  (This should be in a JS file part2-question16.js)
       --- Code Provided ---

17. If the function above is called with the following parameters modifyArray([1,2,3], doSomething), what will be the result? Briefly walk through how you arrived at that result. (This should be in your part2.md). Here we are passing in a function as a parameter, however we can also return a function from another function just as easily, you're encouraged to play around with callbacks as they are used heavily in frontend JS development. 
    This returns [2, 4, 6], this is because each for each value in the array it applies the callback to that elemtn and pushes its value that was multiplied by 2 using doSomthing. 

18.  The above program only prints out the time once when executed. Modify this code such that the program prints out the current time every second.  (This should be a JS file - part2-question18.js)
    --- Code Provided ---

19. What is the output of the above code? (This should be in your part2.md)
    the function printNums() returns the values 
    1
    4
    4
    2