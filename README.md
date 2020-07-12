# C++ Reference Cheat-Sheet

## Common Data Types

|**data type**|**bits** |**Range**|
|:-------:|:--------:|:--------:|
|`int`|32-bits| -2,147,483,647 to 2,147,483,647|
|`int_64`|64-bits|9,223,372,036,854,775,807|
|`INT_MAX`|32-bits| 2,147,483,647 (*constant*)|
|`INT_MIN`|32-bits| -2,147,483,647 (*constant*)|
|`char`|8-bits, 1-byte| -127 to 127|

------------------------------
## Useful Tips
### 1. To check for Integer overflow
#### Steps:-
+ we have to define `#define INT_MIN (-INT_MAX-1)` due to this [Stack-Overflow-Boolean-Issue.](https://stackoverflow.com/questions/14695118/2147483648-0-returns-true-in-c)
+ check if the result is getting overflow using this parameter `if(result>INT_MAX/10 || result<INT_MIN/10) return false` or `return 0`.

----------------------------

## String Functions

|Function | Description | Output|
|:----- | :------| :-----:|
|`strcpy(s1,s2)`| copies string s2 into s1 |" " ,"World"|"World"|
|`strcat(s1,s2)`|


# 
