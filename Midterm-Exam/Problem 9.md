Write a function to flatten a list. The list contains other lists, strings, or ints. For example, ```[[1,'a',['cat'],2],[[[3]],'dog'],4,5]``` is flattened into ```[1,'a','cat',2,3,'dog',4,5]``` (order matters).
```python
def flatten(aList):
    ''' 
    aList: a list 
    Returns a copy of aList, which is a flattened version of aList 
    '''
```


_Hint: How to think about this problem_
>Recursion is extremely useful for this question. You will have to try to flatten every element of the original list. To check whether an element can be flattened, the element must be another object of type list.

```python
def flatten(aList):
    output = []
    
    for element in aList:
        if not isinstance(element, list):
            output.append(element)
        else:
            output.extend(flatten(element))

    return output
```
