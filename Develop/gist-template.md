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

Did not use any quantifiers for this tutorial but here are some common qunatifiers that are usually in regular expressions:

'*': Matches zero or more occurrences of the preceding character or group.

'+': Matches one or more occurrences of the preceding character or group.

'?': Matches zero or one occurrence of the preceding character or group.

'{n}': Matches exactly n occurrences of the preceding character or group.

'{n,}': Matches at least n occurrences of the preceding character or group.

'{n,m}': Matches between n and m occurrences of the preceding character or group.



### OR Operator

Did not use any OR Operators

If i did, 'cookie|monster': Matches either "cookie or "monster". or
cookie|book|milk: matches either "cookie, "book", "milk.

### Character Classes

'\b': Matches a word boundary, which is the position between a word character (as defined by \w) and a non-word character (as defined by \W), or the start or end of a string. In this regex, \b is used to ensure that the words "cookie", "flour", "sugar", and "butter" are matched as whole words, not as parts of longer words.

'\w': Matches any word character, which includes letters, digits, and underscores. In this regex, \w is used in the positive lookahead assertions to match any sequence of word characters that contains the specified words.

'\W': Matches any non-word character, which includes spaces, punctuation, and other non-alphanumeric characters. In this regex, \W is used in the positive lookahead assertions to match any sequence of non-word characters that separates the specified words.

'.': Matches any character except a newline character. In this regex, .* is used at the end of the pattern to match any number of characters (including spaces and other non-word characters) between the specified words

Using the characters allowed me to match a range of input strings and seperate the words "cookie", "flour", "sugar" and butter.

### Flags

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
