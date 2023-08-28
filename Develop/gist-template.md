# Mastering Regular Expressions: A Comprehensive Guide

Welcome to the Mastering Regular Expressions tutorial! In this guide, we'll dive into the world of regex and explore its various components, helping you become proficient in using regular expressions for pattern matching and manipulation of text.

## Summary

In this tutorial, we'll focus on understanding and using the following regex pattern that matches email addresses:

regex
^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$

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
- [Author](#author)


## Regex Components

### Anchors

Anchors are regex elements used to match specific positions within the text. Here are two commonly used anchors:

^ (Caret): Matches the start of a line.
$ (Dollar Sign): Matches the end of a line

^Start 
End$

### Quantifiers

Quantifiers control the number of times a preceding element should occur. Here are a few examples:

*: Matches zero or more occurrences.
+: Matches one or more occurrences.
?: Matches zero or one occurrence.

code:

\d+
[a-z]*

### OR Operator

The OR operator | allows you to match either of two alternatives. For instance, (cat|dog) will match either "cat" or "dog". This is useful when you're looking for multiple possible patterns.

### Character Classes

Character classes let you match specific sets of characters. examples:

[aeiou]: Matches any vowel.
[0-9]: Matches any digit.
\d: Matches any digit (shortcut).

[aeiou]
[0-9]

### Flags

Flags modify how regex patterns are matched. Common flags include i for case-insensitive matching, g for global matching, and m for multiline matching. Flags allow you to customize the behavior of your regex patterns.

### Grouping and Capturing

Parentheses () are used for grouping and capturing parts of a pattern. They allow applying quantifiers to a group. Captured groups can be referenced later.

(a|b)+
(\d{2,4})-(\d{2})-(\d{2,4})

### Bracket Expressions

Bracket expressions define a set of characters enclosed within square brackets. They allow you to match any one character from the defined set. For example, [aeiou] matches any vowel.

### Greedy and Lazy Match

By default, quantifiers are greedy, meaning they match as much text as possible. Adding a ? after a quantifier makes it lazy, causing it to match as little text as possible. This is useful when you want to match the shortest possible string.

### Boundaries

Boundary assertions like \b match positions where a word starts or ends. They are useful for ensuring that a pattern occurs at word boundaries and doesn't match within larger words.

### Back-references

Back-references allow referring to previously captured groups. They're useful when searching for repeated patterns.

(\w)\1

### Look-ahead and Look-behind

Look-ahead (?=...) and look-behind (?<=...) assertions let you assert that a pattern is or isn't followed by or preceded by another pattern, respectively. They don't consume characters, making them useful for complex conditions.


## Author

This guide was created by [Isaiah Jordan](https://github.com/Ijordan4). If you have any questions or suggestions, feel free to reach out on GitHub. Happy regex matching!
