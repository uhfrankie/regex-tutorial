# Regular Expressions

Regular expressions, or regex, are a set of characters used to define a pattern for searching text. they are widely used for text processing and pattern matching. This README covers the various lements that form regukar expressions.

## Summary

This code snippet with demonstrate a regular expression that verifies whether a string matches the structure of an email address:
    `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

    ^ - Matches the beginning of the input string
    ([a-z0-9_.-]+) - Matches one or more characters that can be lowercase letters, digits, underscores, hyphens, or periods, and captures them in a group
    @ - Matches the '@' symbol
    ([\da-z.-]+) - Matches one or more characters that can be lowercase letters, digits, hyphens, or periods, and captures them in a group
    . - Matches a literal period (.)
    ([a-z.]{2,6}) - Matches two to six characters that can be lowercase letters or a period, and captures them in a group
    $ - Matches the end of an input string



## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

## Regex Components
Regular expressions, or regex, are a set of characters used to define a pattern for searching text. they are widely used for text processing and pattern matching. This README covers the various lements that form regukar expressions.

### Anchors
Anchors define the position of a match in a string. They represented by the caret (^) and dollar sign ($). Here's some examples of anchors:

    ^ (caret): matches that start of a string
    $ (dollar sign): matches the end of a string

### Quantifiers
Quantifiers specify the number of times a character or group should match. They are indicated by curly brackets {}. Here's some examples of quantifiers:
    {x}: matches the mentioned character x times
    {x, }: matches the mentioned character at least x times
    {x,y}: matches the mentioned character between x and y times

### Bracket Expressions
Bracket expressions, also known as character classes, allow you to match any one character from a set of characters in a regular expression. A bracket expression is encloses in square brackets [] and contains a list of characters ranges that you want to match.

### Character Classes
A character class is a set of characters enclosed in square brackets [] that matches any one character from that set. Here's some common character classes and what they match:
    [a-z]: matches any lowercase letter from a to z.
    [A-Z]: matches any uppercase letter from A to Z.
    [0-9]: matches any digit from 0 to 9.
    [a-zA-z]: matches any letter, regardless of case.
    [\d]: matches any digit character.
    [\D]: matches any non-digit character.
    [\s]: matches any whitespace character, including spaces, tabs, and line breaks.
    [\S]: matches any non-whitespace character.


### The OR Operator
The OR operator combines two or more conditions or expressions and returns true if at least one of the conditions is true. Here's how it works:
    If both expressions are true, the OR operator returns true.
    If only one expression is true, the OR operator returns true.
    If both expressions are false, the OR operator returns false.

### Flags
Flags are optional parameters that modify how the pattern is matched when added to the end of the expressions.
    g (global): This flag finds all matches in the input string instead of stopping after the first match.
    i (ignore case): This flag ignores the difference between uppercase and lowercase letters when matching.
    s (dotall): This flag causes the "." metacharacter to match any character, including line breaks.
    u (unicode): This flag flag enables support for Unicode characters in the regular expression.

### Character Escapes
Character escapes consist of two or more characters and are used in many programming languages, data formats, and communicating protocols. They are initiated by an escape character, which indicates that the following characters should be interpreted differently than if they were not part of an escape sequence.
    JavaScript uses the backslash \ as an escape character for: [1][2]
        \' single quote
        \" double quoate
        \\ backslash
        \n new line
        \r carriage return
        \t tab
        \b backspace
        \f form feed

## Author

If have any questions for me, please [contact me](mailto:frankie01marie@yahoo.com), or on here [GitHub](https://github.com/uhfrankie).
