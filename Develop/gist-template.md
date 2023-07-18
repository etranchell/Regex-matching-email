Regex-matching-email

## Summary

Regex or regular expression is a way to check for valid input. In this tutorial I will show you a regex for checking emails.

^[a-zA-Z0-9_.+-]+@[a-zA-Z0-9-]+\.[a-zA-Z0-9-.]+$

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

Here are the components of the regex for matching emails.
^[a-zA-Z0-9_.+-]+@[a-zA-Z0-9-]+\.[a-zA-Z0-9-.]+$

### Anchors

^ and $

Anchors are used to check for a match at the beginning or end of a line. The ^ is used to check for a match at the beginning of a line. The $ is used to check for a match at the end of a line.

### Quantifiers

- and \*

The + is used to check for one or more of the preceding token. The \* is used to check for zero or more of the preceding token.

### OR Operator

The OR operator '|' is used to check for a match of either the expression before or after the operator. In this case, the OR operator is used to check for a match of either the expression before or after the '@' symbol.

### Character Classes

Character classes are used to check for a match of any character in the brackets.
[a-z] matches any lowercase letter from a to z
[A-Z] matches any uppercase letter from A to Z
[0-9] matches any number from 0 to 9
[_.+-] matches any of the characters in the brackets

### Flags

Flags are used to change the way the regex is interpreted. In this case, the flags are used to ignore case.
Common flags are:
i - ignore case
g - global search (find all matches)
m - multiline search

In matching emails, the i flag is used to ignore case.

### Grouping and Capturing

() are used for grouping. This is used to treat a part of regular expression as a single unit.
Capturing in the case of emails allows you to match specific parts of an email address, ex before of after the @ symbol.

### Bracket Expressions

Bracket Expressions are used to match any character in the brackets
[abc] matches any character in the brackets, matches either 'a' 'b' or 'c'
[^abc] matches any character not in the brackets, matches any character except 'a' 'b' or 'c'

### Greedy and Lazy Match

Greedy match matches as much as possible. Lazy match matches as little as possible.

- is a greedy match as it matches zero or more of the preceding token.
  ? is a lazy match as it matches zero or one of the preceding token.

### Back-references

Back-references are used to match the same text as previously matched by a capturing group. In matching emials, this is used to match the same text before and after the @ symbol.

### Look-ahead and Look-behind

Look-ahead and look-behind are used to match text that is followed or preceded by a specific pattern. In matching emails, this is used to match text that is followed by a specific pattern, in this case the @ symbol.
(?=) is used for positive look-ahead
(?<=) is used for positive look-behind

## Author

This was created by Eric Tranchell. Learn more from the repo on GitHub at https://github.com/etranchell/Regex-matching-email
