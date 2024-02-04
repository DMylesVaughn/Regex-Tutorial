# Title (replace with your title)

This is a tutorial explaining how a specific regular expression (regex) functions by breaking down each part of the expression and describing what it does.

## Summary
The REGEX covered in this tutorial is used to match HEX values.  This is the regular expression:
/^#?([a-f0-9]{6}|[a-f0-9]{3})$/
A Hex code is written in base-16 format using characters from 0-9 and A-F.  The most popular use of the Hex code is to define color values.  It is also used to define locations in memory, represent MAC addresses, and display error messages.
The anchors, qualifiers, OR operators, grouping and capturing, bracket expressions, and greedy and lazy match will be described in more detail in associated contents below.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)

## Regex Components

### Anchors
Anchors by themselves don't match any regular expression. These are used to match a string at a specified location such as the beginning or the end of the string.  Let's look further into anchors.

Anchor: ^ 

    The ^ is an anchor that indicates that the beginning of the string must match the character #. # is used to distinguish a hexadecimal number from a decimal number.

Anchor: $

    The $ is an anchor that applies to the end of the string. So the $ is simply ensuring the pattern at the end of the string matches.

### Quantifiers
Quantifiers specify the number of times the previous character or grouping must match in the string.  These allow a user to more easily match patterns of varying lengths.

Quantifier: +

    The + is a quantifier indicating that the previous character or grouping must occur one or more times.

    The ? is a quantifier indicating that the previous character or grouping is optional and can occur zero or one time.

    The * is a quantifier indicating that the previous character or grouping zero or more times.

    The {n} is a quantifier indicating that the previous character or grouping must match exactly n times.

    The {n,} is a quantifier indicating that the previous character or grouping must match n or more times.

    The {n,m} is a quantifier indicating that the previous character or grouping must match between the two fixed numbers of n and m.

### OR Operator
OR Operators are used to identify either/or of two choices.  These will be located on either side of the OR operator.

OR Operator: |

    The | is an OR operator that means the search will choose all strings that contain either  of the values entered before and after the | OR operator.

### Character Classes
Character classes are used to match one of several defined characters in a set.

Character Classes: - or --

    The character classes are identified by the use of the - or multiple - used in multiple sets of ranges. An example of a multi dash hex string would be a-f0-9.  This indicates a range of zero through nine and a range of 'a' through 'f'.

### Grouping and Capturing
Grouping and Capturing is a method of defining groups of characters and then extract that data for further processing.

Grouping and Capturing: ()

    The () allow all the characters inside to be treated as a singel value.  The group of data will be expressed as an array when it is captured.  

### Bracket Expressions
Bracket expressions are used to match a specific pattern of characters.  In order for this to work, the characters must be placed with brackets.

Bracket Expression: []

    The brackets indicate that a specific pattern of characters or range of characters must be match the search criteria.  An example of this would be [3-7] where the range of characters must match within the range of three through seven.

## Author
Myles Vaughn

    Myles is a manager for a large defense contractor.  He leads a small Software Development Team.  He has enrolled in the Full Stack Web Development Bootcamp in order to gain an understanding of the everyday rigors faced by a software developer.  This experienced has hel him to bond with his team through mutual understanding and appreciation for the skill of software development.

    Github: [DMylesVaughn](https://github.com/DMylesVaughn)


