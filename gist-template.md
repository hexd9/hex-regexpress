# Hex-regexpress

Welcome to this tutorial on regex for password validation! Regular expressions (regex) are tools for pattern matching and validation. In this guide, I'll break down a regex pattern specifically designed for password validation, ensuring that passwords meet certain criteria for security.

## Summary

^(?=._[A-Z])(?=._[a-z])(?=._\d)(?=._[!@#$%^&*]).{8,}$

My regex featured in this tutorial is designed to validate passwords based on the following criteria:

At least 8 characters long
Contains at least one uppercase letter
Contains at least one lowercase letter
Contains at least one digit
Contains at least one special character (e.g., !@#$%^&\*)

## Table of Contents

- [Anchors](#anchors)
- [Look-ahead Assertions](#look-ahead-assertions)
- [Character Classes](#character-classes)
- [Quantifiers](#quantifiers)

## Regex Components

### Anchors

Anchors are used to specify the position of the pattern in relation to a line of text.

(^ and $)

^ : Marks the beginning of the line.

$: Marks the end of the line.

### Look-ahead Assertions

Look-ahead assertions are zero-width assertions that let you test what's to the right of your current position in the string without actually consuming any characters.

(?=.\*[A-Z]): Positive lookahead to ensure at least one uppercase letter is present.

(?=.\*[a-z]): Positive lookahead to ensure at least one lowercase letter is present.

(?=.\*\d): Positive lookahead to ensure at least one digit is present.

(?=.\*[!@#$%^&\*}): Positive lookahead to ensure at least one special character from the set is present.

### Character Classes

Character classes allow you to match any one out of a set of characters.

([A-Z], [a-z], \d, [!@#$%^&*])

### Quantifiers

Quantifiers define how many instances of a character, group, or character class must be present in the input for a match to be found.

.{8,}: Ensures the password is at least 8 characters in length.

## Author

https://github.com/hexd9/hex-regexpress

This tuturiol was created by Hector Delgado, a full stack developer bootcamp student. Dive into my Github profile for more insight on my projects.
