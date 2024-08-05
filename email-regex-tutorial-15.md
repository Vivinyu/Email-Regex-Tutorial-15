# Regex Tutorial: Matching an Email Address

## Introduction

This tutorial explains the regular expression (regex) used for matching email addresses. Understanding this regex will help you validate email inputs in your applications.

## Summary

We'll break down the following regex used to match email addresses:

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)

## Regex Components

### Anchors

- `^` - Matches the start of the string
- `$` - Matches the end of the string

These anchors ensure that the regex matches the entire input string.

### Quantifiers

- `+` - Matches one or more occurrences of the preceding character set
- `{2,6}` - Matches between 2 and 6 occurrences of the preceding character set

### Character Classes

- `\d` - Matches any digit (0-9)
- `.` - Matches any character except newline

### Grouping and Capturing

- `(...)` - Creates a capturing group

There are three capturing groups in this regex:

1. `([a-z0-9_\.-]+)` - Matches the local part of the email
2. `([\da-z\.-]+)` - Matches the domain name
3. `([a-z\.]{2,6})` - Matches the top-level domain

### Bracket Expressions

- `[a-z0-9_\.-]` - Matches any lowercase letter, digit, underscore, dot, or hyphen
- `[\da-z\.-]` - Matches any digit, lowercase letter, dot, or hyphen
- `[a-z\.]` - Matches any lowercase letter or dot

### Greedy and Lazy Match

This regex uses greedy matching by default. The `+` and `{2,6}` quantifiers will match as many characters as possible while still allowing the overall pattern to match.

## Author

This tutorial was created by [Jose De Los Santos Oliver]. You can find more of my work on my [GitHub profile](https://github.com/Vivinyu)
