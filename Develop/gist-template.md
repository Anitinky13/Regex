# Regex Tutorial

## User-Story

"AS A web development student <br>
I WANT a tutorial explaining a specific regex <br>
SO THAT I can understand the search pattern the regex defines."
<br>
In this template, a tutorial is given on regex (Regular Expressions),
_a series of special characters that define a search pattern_. <br>

## Summary

The regex I will be describing here will be going over the expressions on how to validate a users email address. Here is the code snippet that will be used to validate the email address:
`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

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

### Anchors:anchor:

Anchors do not match any character. Instead they match position. They are the symbols that indicate the START and FINISH positions of the regular expressions. In my code snippet, the `^` represents the begining of the text and `$` represents the end of the text.

### Quantifiers

Quantifiers match a number of instances of a character, group or character class in a string.In quantifiers theres `{n}` is the simplest quantfiers. Theres also `+` and `?`. In my snippet we have `{}` and `+`. the `{}` specify the number of instances of a character. the `+` attaches one a regex section to the next part of the sequence. So `/^([a-z0-9_\.-]+` attaches it to this part `)@([\da-z\.-]`.

### OR Operator

There arent any OR operator in my code snippet. But they are there to basically say that characters on the left and right side would pass as a match. For example `|10` would pass as `5` and/or `ten`.

### Character Classes

A character class is a set of characters enclosed within a square brackets.Regex can match only on out of several characters, you would simply just place the characters you need to match between square brackter. You can also use the `-` inside a character class to specify a range of characters like `[0-9]` and you can use more than one range. like in my code snippet we have `[a-z0-9]`. Character classes are one of the most commonly used features in regular expressions. They are very useful. In my code snippet `[a-z0-9_]` it will look for lowercase letters `a to z` and numbers `0,1,2,3,4,5,6,7,8,9`

### Flags

So the regular expressions for consist of patters and option flags `g,i,m,u,s,y`. The `m` is for multiline mode which if was used it would affect the `^` and `$`, The `g` flag is for global search, it matches all occurences .

### Grouping and Capturing

We have `()` `[]` `{}` and `symbols`, the separate the email address into sections, like `(letters and numbers)` `@` `(letters and numbers)` for example like `anasmi45@fake.com` or `3_l577@email.com`. Something that wouldnt match would be an email that has an uppercase letters and too many characters.

### Bracket Expressions

Bracket Expression `[]` it indicates to match whatever is inside of it. we have first set of brackets `[a-z0-9_\.-]` it matchets all the lowercase letters and 0-9 numbers, it also matches an underscore and a hyphen and a period. On the other hand the `{}` they match the exact amount of things. We have `{2,6}` this means there can only be at least 2 and mac of 6 characters in the email.

### Greedy and Lazy Match

Greedy means match the longest possible string, and Lazy means match the shortest possible string. So the regex would match as many characters as posssible or as little as possible.by default the `*` and `+` are greedy. In my code snippet we have the `+` greedy match so it would match as many characters as possible. We do not have a lazy match here but it would probably look something like `+?`.

### Boundaries

Boundaries set the start and end of an expression, and use `\` to excape the characters. We have `a-z0-9` which match lowercase letters and numbers. It would not match an uppercase though.

### Back-references

Back-references are referred to a previous part of a matched regular expressions. usuall specified with a `\2` a backslash and single digit. They are usually used in bigger expressions.

### Look-ahead and Look-behind

The look-behind means to look what is before and look ahead is to look what is after your match.

## Author

My name is Anastasiya Litvinova, A web developer from San Antonio, Tx.
I am currently finishing a full-stqack dev bootcamps and working on becoming employed in front-end and/or back-end.
[ :octocat: Github Profile](https://github.com/Anitinky13)
