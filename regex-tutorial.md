# Regex Breakdown

Regex are handy tools that allow the user to check if a set of characters matches some sort of criteria. In this case we will match to a hexidecimal number which has countless uses

## Summary

This will be a tutorial on how to understand the following regex:

```
/^#?([a-f0-9]{6}|[a-f0-9]{3})$/
```

and each of its components

## Table of Contents

- [Anchors](#anchors)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)

## Regex Components

/

While not an anchor, the regex may be required to be wrapped in slash chars "/" since they are considered literals in some languages.

### Anchors

^

This signifies the beginning of the expression

$

This signifies the end of the expression

### Grouping and Capturing

()

This groups multiple tokens together, in our case it requires the alphanumeric characters to follow the "#" symbol

### Bracket Expressions

[a-f0-9]

This checks if a given character is a-f or 0-9, meaning that any character within the range is acceptable. It is also case sensitive.

### Quantifiers

#?

The ? indicates that the preceding symbol is optional, meaning it requires either 0 or 1. In this case it is the "#" which is commonly used to denote hexidecimal numbers

[a-f0-9]{6}

The {6} indicates that there is exactly 6 of the preceding character, similarly

[a-f0-9]{3}

indicates that there is exactly 3 of the preceding character

### OR Operator

|

This character checks if at least one of the cases matches

```
[a-f0-9]{6}|[a-f0-9]{3}
```

In this case it checks if either [a-f0-9]{6} or [a-f0-9]{3} is satisfied

## Author

This breakdown was created by Christopher Gonzales, a full-stacks bootcamp student, whose other works can be located at: https://github.com/Christophgonz
