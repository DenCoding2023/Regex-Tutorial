# Title (Regex Tutorial: Matching an Email Address)

Introduction:
Welcome to the Regex Tutorial for matching an email address! In this comprehensive guide, we will explore the regular expression /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/ and dissect each component. By the end of this tutorial, you will have a solid understanding of regex anchors, quantifiers, operators, character classes, flags, grouping and capturing, bracket expressions, greedy and lazy matching, boundaries, back references, and look ahead and look behind constructs. You will learn how to create a powerful regular expression to match and validate email addresses, extract them from text, and understand the inner workings of each regex component.

## Summary

This tutorial focuses on a specific Regex Pattern: /^([a-z0-9_.-]+)@([\da-z.-]+).([a-z.]{2,6})$/ We will break down this regex and explain each component to grasp its full functionality.
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
Regex components, also known as regular expression metacharacters or constructs, are the building blocks that form a regular expression pattern. Each component serves a specific purpose in defining the rules for matching and manipulating text patterns. Here are some common regex components:

Literals: These are characters that match themselves literally. For example, the regex a will match the letter "a" in the text.

Metacharacters: Special characters that have a predefined meaning in regex. Some common metacharacters include:

- . (dot): Matches any single character except newline.
- (*) (asterisk): Matches zero or more occurrences of the preceding character.
- (+) (plus): Matches one or more occurrences of the preceding character.
- ? (question mark): Matches zero or one occurrence of the preceding character.
- | (pipe): Acts as an OR operator, matching either the expression on its left or right.
Character Classes: A set of characters enclosed in square brackets [ ]. It matches any single character that is within the class. For example, [aeiou] matches any vowel.

Negated Character Classes: Similar to character classes, but matches any character not present in the set. Represented as [^ ]. For example, [^0-9] matches any non-digit character.

### Anchors
- ^: The caret symbol anchors the match to the start of the text, ensuring the email address is found at the beginning of the string.
- $: The dollar sign anchors the match to the end of the text, ensuring the email address is found at the end of the string.
### Quantifiers
- +: Matches one or more occurrences of the preceding character or group.
- {2,6}: Matches between 2 and 6 occurrences of the preceding character or group.
- *: Matches zero or more occurrences of the preceding character or group.
- ?: Matches zero or one occurrence of the preceding character or group.
### OR Operator
- @: The "@" symbol matches itself, ensuring it exists in the email address.
- .: The backslash is used to escape the dot (.) character, allowing it to match itself. This ensures a dot separates the domain name from the top-level domain.
### Character Classes
- [a-z0-9_.-]: Matches lowercase letters, digits, underscores, dots, and hyphens.
- [\da-z.-]: Matches lowercase letters, digits, dots, and hyphens. "\d" represents any digit character.
### Flags
- Flags are optional modifiers that can be applied to the regex pattern. Common flags include:
- i: Case-insensitive matching.
- g: Global matching (find all occurrences).
- m: Multiline matching.
### Grouping and Capturing
- (): Parentheses group characters or expressions together.
- Capturing groups (e.g., ([a-z0-9_\.-]+)) capture and remember the matched content for later use.
### Bracket Expressions
- [a-z.]: Matches lowercase letters and dots. The dot here is not a metacharacter, so it matches itself literally.
### Greedy and Lazy Match
- By default, quantifiers are greedy and match as much as possible. To make them lazy, add a "?" after the quantifier (e.g., *? or +?).
### Boundaries
- \b: Matches a word boundary, ensuring the email address is a standalone word.
### Back-references
- \1, \2, etc.: Refers back to captured groups. For example, \1 refers back to the first capturing group.
### Look-ahead and Look-behind
- (?=...): Positive lookahead. Matches a group after the main expression without including it in the result.
- (?!...): Negative lookahead. Matches if the group does not follow the main expression.
## Author

This tutorial was created by Dennis Luciano, I am recent student at the fullstack web EX program. You can find moore of my work and contributions on GitHub profile: https://github.com/DenCoding2023/Regex-Tutorial.git
