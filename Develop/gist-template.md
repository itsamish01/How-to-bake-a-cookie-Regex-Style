# Title: How to bake a cookie

1. To start off the tutorial we will need to start the the beginning of the string.
2. Looking ahead in the string for the word "cookie".
3. If "cookie" is found, continue to the next step. Otherwise, backtrack and try again.
4. Look ahead for the string for the word "flour".
5. If "flour" is found, continue to the next step. Otherwise, backtrack and try again.
6. Look ahead in the string for the word "sugar".
7. If "sugar is found, continue to the next step. Otherwise, go back and try again.
8. Look ahead in the string for the word "butter".
9. If "butter" is found, continue to the next step. Otherwise, go back and try again.
10. Make sure to match any remaining characters in the string.
11. End the match at the end of the string.
12. If the entire pattern is found, return a match, If not, then don't return a match. 

## Summary

/^(?=.*\bcookie\b)(?=.*\bflour\b)(?=.*\bsugar\b)(?=.*\bbutter\b).*$/i

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

### Anchors

'^': This anchor denotes the start of the string. In this regex, it is used to ensure that the pattern matches only at the beginning of the string.

'$': This anchor denotes the end of the string. In this regex, it is used to ensure that the pattern matches only up to the end of the string.


### Quantifiers

### OR Operator

### Character Classes

### Flags

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
