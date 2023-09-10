# Title Regular Expressions

This guide will introduce and explain a specific regular expression(regex), it will provide a basic understanding on how a regex can help search patterns.

## Summary

A regular expression(regex) is must start with the `/` character. In this example I will use the regex `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/` to compare and match email addresses.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)

## Regex Components

### Anchors
The characters `^` and `$` are known to be anchors in regular expressions. They behave as the start and end.
- `^` Character acts as the start of a regular expression.
- -`$` Character acts as the end of a regular expression.
### Quantifiers
Quantifiers specify how many times a character must be present in the input for a match to be found. The quantifier can be identified in the example regex towards the end. `([a-z\.]{2,6})$\`. The `anchor` `$` can be seen towards the end. However, the a-z will only be searched in lengths of 2 to 6 characters long.
### Grouping Constructs
Grouping captures patterns within the larger group, this can be referred to as a subpattern. Using `()` will indicate a grouping. Look back at the example regex and see if you can spot a grouping construct.
### Bracket Expressions
Looking for `[]` in the example regex will identify a bracket expression. In the example regex `[a-z0-9_/.-]` is a bracket expression would capture A-Z in lowercase only`a-z`, every number`0-9`, every underscore `_`, every period `.`, and all hyphens `-`
### Character Classes
Character classes define sets of characters. There are a vast amount of character classes. I will introduce a few, and also link documentation for a more in-depth look inside `Character Classes`.
`/w` Will match any alphanumeric character: A-Z, a-z, 0-9.

`/s` Will match any single white space character. These include simple spaces, tabs, and more.

`/d` Will match any digit.

Here is documentation to read further into `Character Classes` 

`https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_expressions/Character_classes`.
### The OR Operator
The `|` character symbolizes an `OR` character. This allows you to find certain sequences of characters. 

For example: `abc|xyz` would search for abc or xyz respectively.
### Flags
Regular expressions can include flags that will affect the search. There are 6 flags in JavaScript.

`i` This flag indicates that the search will be case-insensitive.

`g`  This flag will search for all matches included.

`m` This flag will search multiple lines

`s` This flag will allow a `.` to match a newline.

`u` This flag will enable full Unicode support.

`y` This flag will search at an exact position.


## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
