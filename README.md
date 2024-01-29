# Title: THregex

This tutorial explains how a specific regular expression, or regex, functions by breaking down each part of the expression and describing what it does.

## Summary
JavaScript has many useful methods that can check if a string contains a certain letter or phrase. Regular Expression or Regex is one of them, which represents a seriese of special characters that define a search pattern.

For this challenge, I chose to explain the given
````
Matching a URL – /^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/
````
and the detail descriptions are provided below.
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
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)
- [References](#references)

## Regex Components

### Anchors
 - There are two types of "Anchors". The caret(^) and dollar($)
 - Meta-character ^ represents the starting position of the string and 
 - Meta-character $ represents the ending position of the string.
 - For example,  /^#?([a-f0-9]{6}|[a-f0-9]{3})$/ represents a Hexadeciamal value.
 
### Quantifiers
 - Regex provides a variety of quantifiers that one can use to match the sequesnce.
 - The * quantifier represents, zero or more occurences of the pattern.
 - The + quantifier represents, one or more occurences of the pattern.
 - The ? quantifier represents, zero or one occurance of any character.
 - The bracket quantifier consists of a pair of curly braces, like {}, containing one or two numbers with an optional comma between the braces:
 - - p{m} matches precisely m occurrences of the pattern p.
 - - p{m,} matches m or more occurrences of p.
 - - p{m,n} matches m or more occurrences of p, but not more than n.
 - The quantifiers are always applied to only one pattern, the one it finds to the left of the quantifier. 
 
### OR Operator
 - Regex has a "Logical OR" operator known as "the pipe".
 - It simply means this or that.
 - For example, 'The petshop have (cats|dogs)'
 
### Character Classes
 - Character class in regular expression represents set of characters, any one of which can occur in an input string to fullfill matching requirement. Some common character classes are:
 - \d is equivalent to [0-9], matches any numeric digit.
 - . matches any character except the new line 
 - \n matches new line
 - \w matches any alpha numeric character, equivalent to [A-Z0-9a-z_]
 - \s matches single whitespace including tabs and line break.
 - \D matches non-digit character.

### Flags

### Grouping and Capturing

### Bracket Expressions
 - Anything inside a set of square brackets ([]) represents a range of characters that must be matched. These patterns are known as bracket expressions
 - For example, [a-z] will look for a match that includes any alphabet between a and z.
 - Similarly, [a-z0-9_-], this will match any string that includes any combination of lowercase letters between a and z, any number between 0 and 9, and the special characters of an underscore or a hyphen.
 
### Greedy and Lazy Match

### Boundaries

### Look-ahead and Look-behind

### References
- JavaScript Regular Expression: [ https://www.w3schools.com/jsref/jsref_obj_regexp.asp ]
- Regex Quickstart Cheatsheet: [ https://www.rexegg.com/regex-quickstart.html ]
- MDN Web Doc Regex : [ https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/RegExp ]
- Regular Expression Cheatsheet by Vitor Britto: [ https://gist.github.com/vitorbritto/9ff58ef998100b8f19a0 ]

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)