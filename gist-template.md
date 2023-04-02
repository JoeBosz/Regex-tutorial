# Title (replace with your title)

Introductory paragraph (replace this with your text)

## Summary

Matching A email adress with regex: 

The following regex can be used to verify that user input is a valid email address

```
/^[a-z0-9_\.+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/s
```
Each component of this specific regex have a responsibiliy to make sure the user enters in a email hat begins with unspecified number of chracters  preceding the @ symbol, followed by a domain name. The domain name must conainat least one period. the domain name must also end with a valid top-level domain, such as .com, .net or .org. 

Characters are the simplest in regex. They match themselves 1 for 1. For example, the Regex /abc/ matches the string abc

Meta characters how ever are chacers that do not match themselves as literals. Instead they are seen as commands that tell regex engines to perform a more complex or refiend search meta characters inculde the following. 

- . (period) - matches any single character except the newline character
- \w - matches any word character (alphanumeric character plus underscore) 
- \W - matches any non-word character
- \d - matches any digit
- \D - matches any non-digit character
- \s - matches any whitespace character (space, tab, newline, and return)
- \S - matches any non-whitespace character
- \b - matches the empty string, but only at the start or end of a word
- \B - matches the empty string, but not at the start or end of a word
- \0 - matches the null character
- \n - matches a new line character
- \t - matches a tab character
- \v - matches a vertical tab character
- \f - matches a form feed character
- \r - matches a carriage return character
- \xhh - matches the character with the hexadecimal value hh
- \uhhhh - matches the character with the hexadecimal value hhhh
- \cX - matches the control character indicated by X


## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

## Regex Components

### Anchors

Anochors are used to match a pattern at the beginning or end of a string. The ^ symbol is used to match the beginning of a string, and the $ symbol is used to match the end of a string. Anchors are a different breed from literal and meta characters, because they do not match a single character. Instead, they match the position before, after, or between characters. So, applying ^a to abc matches a. ^b does not match abc, because b is not at the beginning of the string.

Similarly, $ matches right after the start of the string. So, applying c$ to abc matches c. Applying a$ to abc does not match, because a is not at the end of the string.

Check Your Understanding:

^ signifies a string that begins with characters that match the pattern that follows the ^ symbol.
$ signifies a string that ends with characters that match the pattern that precedes the $ symbol.

A regex that consists soley of an anchor can only find zero-length matches. This can be useful, but can also create complications.


### Quantifiers

Quantifiers in regex are operators that connect the users email name to the domain name to the top-level domain. A regex quantifier includes + and in this case {2,6}. The + quantifier matches one or more of the preceding token. The {2,6} quantifier matches between two and six of the preceding token.

{2,6} will allow a match of any string that contains at least two characters and at most six characters. For example, the regex /a{2,6}/ matches the string aaaaaa, but not the string a.
s

### Grouping Constructs

### Bracket Expressions

### Character Classes

### The OR Operator

### Flags

### Character Escapes

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
