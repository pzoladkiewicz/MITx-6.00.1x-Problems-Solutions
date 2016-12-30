Implement a function called closest_power that meets the specifications below. 
For example,

    closest_power(3,12) returns 2
    closest_power(4,12) returns 2
    closest_power(4,1) returns 0

Paste your entire function, including the definition, in the box below. Do not leave any debugging print statements.

```py
def closest_power(base, num):
    
    #define spare variables
    exp = 0
    check = 0
    #convert to int
    num = int(num)

    while output < num:
        check = base ** exp
        beforeInc = num - base ** exp
        afterInc = num - base ** (exp + 1)
        if abs(afterInc) >= beforeInc:
            return exp
            
        exp += 1
```
