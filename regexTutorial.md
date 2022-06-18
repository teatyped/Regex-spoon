# Regex explanation for validation of email address

## Summary

Tutorial explaining the different regex components  for email validation .

````
/^[a-zA-Z0-9.!#$%&’*+/=?^_`{|}~-]+@[a-zA-Z0-9-]+(?:\.[a-zA-Z0-9-]+)*$/

````

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Escaped Character](#escaped-Character)


## Regex Components

````
Component Explanation for [a-z0-9_\.-] 

- matches all lowercase characters from a to z
- matches all numeric characters from 0 to 9
- matches special characters such as `_`, `-`, and `.`

````
````
Component Explanation for [\da-z\.-]

- `\d` matches for any decimal digit
- matches all lowercase characters from a to z
- matches special characters such as `.` and `-`
````
````
Explanation for [a-z\.]

- matches all lowercase characters from a to z
- matches special character, `.`
````


### Anchors
- ````^ $ ````     Start / end of the string
- ````\b\B````	    word, not-word boundary

### Quantifiers
- ````a*a+a?````	   0 or more, 1 or more, 0 or 1
- ````a{5}a{2,}	````   exactly five, two or more
- ````a{1,3}````	    between one & three
- ````a+?a{2,}?	````    match as few as possible
- ````ab|cd	 ````       match ab or cd

### OR Operator

### Escaped Character
- ````\.\*\\ ```` escaped special characters
- ````\t\n\r````    Tab, linefeed, carriage return


## Author

Khai Truong
