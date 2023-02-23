# Regex Tutorial

Regex, short for regular expression is a sequence of characters that is used to specify the search patterns in text.  In this .md file, we will go over the componenents of the regular expression.

## Summary



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
Chatacters "^" and "$" are considered anchors. 

"$" signifies a string that ends with characters that precede it.

"^" is like "$", but can also be preceded by an exact string or range of possible matches.  

exact string match ^The matches "The" and "The thing" but not "the" or "the thing". is case sensitive.

ranges can be specified by putting them in "[]", "[abc]" matches "aaa" "bbb" "ccc" "banana" and anything that contains lowercase letters a b or c.  
more in [Bracket Expressions](#bracket-expressions)

### Quantifiers
Quantifiers sets the limits of the string that regex matches. which can include minimum and maximum number of characters that regex is looking for.

- "*" matches pattern zero or more times

- "+" matches patter one or more times

- "?" matches pattern zero or one times. 

- {} can provide 3 different ways to set limits:

  {x} matches the pattern exactly x number of times.

  {x,} matches the pattern at least x number of times

  {x,y} matches the pattern a minimum number of x times to the maximum of y times.

  inherently quantifiers are greedy, meaning the match as many occurrences of the particular patterns as possible, but can be made lazy by adding a ? after it meaning it will match as few as possible.

### OR Operator
(|) is an or operator. (a|b|c):(x|y|z) would match "abc:xyz" and "acb:xyz", as well as "a:z", but "xyz:abc" would not.

### Character Classes



### Flags

### Grouping and Capturing

### Bracket Expressions
is anything inside of square brackets []

[abc] = "aaa", "bbb", "ccc", "banana" and anything else that contains lowercase abc in some way. 

[ABC] = "AAA", "BBB", "CCC", "BANANA" and anything else that contains upercase ABC in some way. 

to do both lower and upper you would have to do [abcABC] and for the full alphabet you could do [a-zA-Z]

it can also contain numbers [0-9] = "hi-5" and anything else with numeric characters. 

can also contain hyphen and underscors [_-] = "hi-5" because is contains a hyphen. "you_suck" would also work. 

adding ^ inside of the brackets would turn it into a negative character group. [^qwerty] would look for matches that do not contain those letters.

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
