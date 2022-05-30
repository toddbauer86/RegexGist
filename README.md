# Regex Tutorial for matching an email

Regex can be confusing to understand but a powerful tool when utilized correctly. There are some difficult concepts to master but ther results are rewarding. This example matches an email address.

## Summary

I will be explaing the following regex expression:
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)

## Regex Components

### Anchors

There are 2 anchors in this example: ^ and $. ^ indicates where the expression starts,and $ indicates where the expression ends.

### Quantifiers

A quantifier specifies how many instance of a character, group, or character class must be present in the input for a match to be found. In this instance, there is a +, which is a greedy quantifier. The {2,6} in the expression indicates that the input must be at least 2 but not more than 6 characters.

### Grouping and Capturing

There are three sets of data being matched in the group. [a-z0-9_\.-] is the unique username of the email address. [\da-z\.-] is for the domain name, and [a-z\.] is for the the extension (ex, .com, .net).

### Bracket Expressions

There are 3 sets of information within their own brackets [].

### Greedy and Lazy Match

There are only greedy matches in this expression. These are + and {}. Lazy matches would contain a ?.

### Boundaries

The boundaries of this expression are identified by ^ and $.

## Author

My name is Todd Bauer and my github is https://github.com/toddbauer86
