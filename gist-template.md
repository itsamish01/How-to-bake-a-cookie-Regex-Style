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

'i': This flag makes the regular expression case-insensitive, so that it matches both uppercase and lowercase letters. In this regex, the i flag is used at the end of the pattern to ensure that the words "cookie", "flour", "sugar", and "butter" can be matched regardless of their capitalization.

### Grouping and Capturing

Did not provide grouping or capturing in my regex snippet but,

Grouping and capturing are typically used in regular expressions to capture specific parts of a matching string, which can then be used for further processing or output. In JavaScript, for example, grouping and capturing can be done using parentheses, like this:

const myRegex = /(\d+)-(\d+)/;
const myString = "123-456";
const myMatch = myString.match(myRegex);
console.log(myMatch[1]); // Output: "123"
console.log(myMatch[2]); // Output: "456"


### Bracket Expressions

 '[]' bracket expressions are used to match any character within a specific set of characters. The [ ] notation is used to define a character set, and any character within the set will be matched by the regular expression.

### Greedy and Lazy Match

Did not provide Greedy and Lazy Match in my regex snippet.

Greedy and lazy matching are concepts used in regular expressions to control how much input is consumed by a pattern match. In a greedy match, the pattern will match as much of the input as possible, whereas in a lazy match, the pattern will match as little as possible.

'/a+/': greedy match, matches one or more "a" characters
'/a+?/': lazy match, matches the smallest possible sequence of "a" characters

### Boundaries

The caret '^' matches the start of the string or line.
The dollar sign '$' matches the end of the string or line.

### Back-references

Did not provide Back-references in my regex snippet but:

Back-references are a feature of regular expressions that allow you to reference a previously matched group within the same regular expression. This can be useful for matching patterns that occur multiple times within the same string.

### Look-ahead and Look-behind

Did not provide Look-ahead and Look-behind in my regex snippet but:

Look-ahead and look-behind are advanced features of regular expressions that allow you to match patterns based on what comes before or after a certain point in the string, without actually including those characters in the match.

## Author

As a seasoned sales and marketing professional with 5 years of experience in the industry, I have a proven track record of success in driving growth and innovation. My passion for technology has led me to learn several technical skills including HTML, CSS, JavaScript, Express, MySQL and Git, which I believe will be invaluable assets in the tech industry.

I am confident in my ability to make a difference in the tech industry and bring a fresh perspective to the table. My experience in sales and marketing has equipped me with strong communication skills, the ability to work collaboratively with teams, and a deep understanding of customer needs.

I am excited to apply my skills and knowledge to the tech industry, and I believe that my background in sales and marketing, coupled with my technical expertise, will enable me to make a significant impact in this rapidly evolving field.
