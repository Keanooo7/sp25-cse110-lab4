1. What is printed by line 9? If the code returns an error, explain why. ^^^^^
    values added:  20

2. What is printed by line 13? If the code returns an error, explain why. 
    final result:  20

3. Why should you not use var? Explain why. 
    Var provies variables with a function scope so that means that regardless of what block it is defined in, it can still be accessed anywhere inside the function it was defined in. This can cause naming conflicts and scopiong issues

4. What is printed by line 9? If the code returns an error, explain why. ^^^^^
    values added:  20

5. What is printed by line 13? If the code returns an error, explain why. 
    Since line 13 is after the closing } for the if statement (block), result goes out of scope so there is no result variable anymore to acsess which is why it gives a RefrenceError

6. What is printed by line 9? If the code returns an error, explain why. ^^^^^
    This line returns a TypeError because you cant reassing a const variable because it is only readable. 

7. What is printed by line 13? If the code returns an error, explain why. 
    Again nothing is printed because a refrence error is given(if line 7 is removed, else it just stops at the reassignment error), since result was declared within the if block trying to accsess it outside will thorw a refrence error because result is no longer defined