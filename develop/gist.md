# CSS rgb & rgba Validator 

This gist provides a breakdown of a regular expression designed to match CSS `rgb()` and `rgba()` color definitions. Both color definitions are used widely in web development, with `rgba()` providing an alpha channel to control opacity. 

## Summary

The regex prov

here is the regex 
```
^(rgb\(\s*(\d{1,3})\s*,\s*(\d{1,3})\s*,\s*(\d{1,3})\s*\)|rgba\(\s*(\d{1,3})\s*,\s*(\d{1,3})\s*,\s*(\d{1,3})\s*,\s*(0|1|0?\.\d{1,2})\s*\))$
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

### Anchors
`^` and `$` are used at the start and end so that the entire string matches the pattern.

### Quantifiers
The `\d{1,3}` is used to check the numbers are between 1 to 3 digits long. <br>
The `\s` allows for zero or more whitespace characters (spaces).

### OR Operator
The `|` is used to separate the `rgb` and `rgba` patterns. It matches either an `rgb()` pattern without an alpha channel or an `rgba()` pattern with an optional alpha channel.

### Character Classes
the `\d` is used to match any digit from 0 through 9.

### Flags
This regex doesn't use any specific flags. 

### Grouping and Capturing
The `(...)` constructs create capture groups. 

### Bracket Expressions
This regex doesn't use any specific Bracket Expressions.

### Greedy and Lazy Match
This regex doesn't use any specific Greedy or Lazy Matches.

### Boundaries
This regex doesn't use any specific word or other boundary matchers.

### Back-references
This regex doesn't use any specific back-references.

### Look-ahead and Look-behind
This regex doesn't use any specfic look-ahead or look-behinds. 

## Author

Bryan Bickel. Please reach out with any questions or suggestions regaurding this regex.
