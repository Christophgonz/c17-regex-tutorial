# Regex Breakdown

intro paragraph

## Summary

This will be a tutorial on how to understand a regular expression, also known as regex. The following regex is one that is commonly used to match to a hexidecimal number:

```
/^#?([a-f0-9]{6}|[a-f0-9]{3})$/
```

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

/

While not an anchor, the regex may be required to be wrapped in slash chars "/" since they are considered literals in some languages.

### Anchors

^

This signifies the beginning of the expression

$

This signifies the end of the expression

### Quantifiers

#?

The ? indicates that the preceding symbol is optional, in this case the "#" which is commonly used to denote hexidecimal numbers

### OR Operator

|

This character checks if at least one of the cases matches

```
[a-f0-9]{6}|[a-f0-9]{3}
```

In this case it checks if either [a-f0-9]{6} or [a-f0-9]{3} is satisfied

### Character Classes

### Flags

### Bracket Expressions

## Author

This breakdown was created by Christopher Gonzales, a full-stacks bootcamp student, whose other works can be located at: https://github.com/Christophgonz
