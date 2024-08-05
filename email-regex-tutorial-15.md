# Regex Tutorial: Matching an Email Address

## Introduction

This tutorial explains the regular expression (regex) used for matching email addresses. Understanding this regex will help you validate email inputs in your applications.

## Summary

We'll break down the following regex used to match email addresses:

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

## Table of Contents

* [Anchors](#anchors)
* [Quantifiers](#quantifiers)
* [OR Operator](#or-operator)
* [Character Classes](#character-classes)
* [Flags](#flags)
* [Grouping and Capturing](#grouping-and-capturing)
* [Bracket Expressions](#bracket-expressions)
* [Greedy and Lazy Match](#greedy-and-lazy-match)
* [Boundaries](#boundaries)
* [Back-references](#back-references)
* [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

### Anchors

1. `^` - Matches the start of the string
2. `$` - Matches the end of the string

These anchors ensure that the regex matches the entire input string.

### Quantifiers

1. `+` - Matches one or more occurrences of the preceding character set
2. `{2,6}` - Matches between 2 and 6 occurrences of the preceding character set

### OR Operator

The OR operator `|` is not used in this email regex, but it's commonly used in other regex patterns to match one pattern or another.

### Character Classes

1. `\d` - Matches any digit (0-9)
2. `.` - Matches any character except newline

### Flags

This regex doesn't use any flags, but common flags include:

1. `i` - Case-insensitive matching
2. `g` - Global matching
3. `m` - Multi-line matching

### Grouping and Capturing

1. `(...)` - Creates a capturing group

There are three capturing groups in this regex:

1. `([a-z0-9_\.-]+)` - Matches the local part of the email
2. `([\da-z\.-]+)` - Matches the domain name
3. `([a-z\.]{2,6})` - Matches the top-level domain

### Bracket Expressions

1. `[a-z0-9_\.-]` - Matches any lowercase letter, digit, underscore, dot, or hyphen
2. `[\da-z\.-]` - Matches any digit, lowercase letter, dot, or hyphen
3. `[a-z\.]` - Matches any lowercase letter or dot

### Greedy and Lazy Match

This regex uses greedy matching by default. The `+` and `{2,6}` quantifiers will match as many characters as possible while still allowing the overall pattern to match.

### Boundaries

The `^` and `$` anchors act as boundaries in this regex, ensuring the pattern matches the entire input string.

### Back-references

Back-references are not used in this email regex, but they allow you to refer to previously captured groups within the regex.

### Look-ahead and Look-behind

Look-ahead and look-behind assertions are not used in this email regex, but they allow you to match a pattern only if it's followed by or preceded by another pattern, without including the latter in the match.

## Author

This tutorial was created by Jose De Los Santos Oliver. You can find more of my work on my [GitHub profile](https://github.com/Vivinyu).
