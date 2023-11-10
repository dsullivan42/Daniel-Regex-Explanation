# Matching a URL

A regex (regular expression) is a sequence of characters that are used to define search patterns. These can be a single character, or a multi character complicated pattern. When implemented into code, we can use regex to find patterns of characters within a string, split a string into an array of substrings, or replace a matched substring with a replacement substring. A common use for these regex, are for validation for user inputs. Overall, regex are extremely useful tools, for coders to utilize within their code. 

## Summary

The regex that I will be using today, will be matching a URL, or, `/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/`. Regex can be used in this case, for the validation in the format. When user's input the URL, the regex will work in ensuring that the url formatting for the web address, is valid. 

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
The anchor tags used in this regex, are the caret (^), which is read as the beginning of the string and the dollar ($) which is read as the end of that string. As you can see in the Regex linked above, it begins with /^ and ends with $/, signifying the beginning and end of the url string.
### Quantifiers
The first quantifier that we utilize in this regex is the question mark(?) which means that it matches the pattern 0-1 times within the string.The next, the plus(+) meaning that the pattern matches 1 or more times. The next, the curly brackets({}) allows you to search for a pattern between a set parameter of numbers, for example, ours is {2,6}, so we are looking for a minumum of 2 matches, and a maximum of 6. The last quantifier that we use in this regex is the star (*), which means that it matches the pattern 0 or more times. 
### Grouping Constructs
Using the parentheses, we can separate the regex, into sections, allowing us to to search for different patterns throught the url, using the regex. We utilize the ?: which makes the grouping construct non-capturing. We use this, in the (https?:\/\/) portion of the code. 
### Bracket Expressions
Bracket expressions, are the expressions within the square brackets of a regex, when matching a url, these include [a-z] which is looking for a single character match in the range of a-z. 
### Character Classes
The character classes, are sets of characters that the regex looks for to fulfill a match. The character classes we use are the \d, which is looking for a match, of a single digit, and the \w, which is looking for a match of any alphanumeric character plus underscore. 
### The OR Operator
We don't make use of the OR Operator with our regex
### Flags
We don't make us of Flags with our regex
### Character Escapes
We make use of Character Escapes for when we use \/, since the forward slash has a special meaning, you need to use the back slash to escape it, to match a literal forward slash. This is the same for the \. and \:,  since . and : are special characters, you need to use \ to match a literal ":" and ".".
## Author

Daniel Sullivan, Coding Bootcamp Student
https://github.com/dsullivan42
