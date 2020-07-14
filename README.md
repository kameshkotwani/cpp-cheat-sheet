# C++ Reference Cheat-Sheet

## Common Data Types

|**data type**|**bits** |**Range**|
|:-------:|:--------:|:--------:|
|`int`|32-bits| -2,147,483,647 to 2,147,483,647|
|`INT_MAX`|32-bits| 2,147,483,647 (*constant*)|
|`INT_MIN`|32-bits| -2,147,483,647 (*constant*)|
|`char`|8-bits, 1-byte| -127 to 127|

------------------------------
## Useful Tips
### 1. To check for Integer overflow
#### Steps:-
+ we have to define `#define INT_MIN (-INT_MAX-1)` due to this [Stack-Overflow-Boolean-Issue.](https://stackoverflow.com/questions/14695118/2147483648-0-returns-true-in-c)
+ check if the result is getting overflow using this parameter `if(result>INT_MAX/10 || result<INT_MIN/10) return false` or `return 0`.

#### To check how much time the execution took place:
+ Add this code snippet at the end of `main` function: `cerr<<"time taken : "<<(float)clock()/CLOCKS_PER_SEC<<" secs"<<"\n";`

----------------------------

## String Functions

|Function | Description |
|:----- | :------|
|`strcpy(s1,s2)`| copies string s2 into s1 |
|`strcat(s1,s2)`| concatenates strings s1 and s2 into s1 |

-----------------------------
## Math Functions

|Function | Description |
|:----- | :------|
|`double cos(double)`|Takes an angle (as a double) and returns the cosine.|
|`double sin(double)`|Takes an angle (as a double) and returns the sine.|
|`double tan(double)`|Takes an angle (as a double) and returns the tangent.|
|`double log(double)`|Takes a number and returns the natural log (base-e) of that number.|
|`double pow(double)`|The first is a number you wish to raise and the second is the power youwish to raise it to.|
|`double sqrt(double)`|Returns square-root of the number.|
|`int abs(int)`| Returns the absolute value. |
|`double fabs(double)`| Returns the absolute value of any decimal number. (eg, 1,1.56,-3.99).|
|`double floor(double)`|Returns the number less than or equal to the number passed.|

--------------------------
## STL Containers and Functions
