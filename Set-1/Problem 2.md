Assume s is a string of lower case characters.
Write a program that prints the number of times the string 'bob' occurs in s.
For example, if s = 'azcbobobegghakl', then your program should print
Number of times bob occurs is: 2
```python
s = 'azcbobobegghbobakl'

string = 'bob'
stringCount = 0
stringLength = len(string)
sLength = len(s)

for n in range (sLength-stringLength+1):
	partOfS = (s[n:n+stringLength])
	if string == partOfS:
		stringCount += 1
print(stringCount)
```
