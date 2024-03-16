# Regex-Tutorial

A regular expression (Regex) is a special text string for describing a search pattern. As a web development student, I would like a tutorial explaining a specific regex so that I can understand the search pattern it defines.

## Summary

I will be explaining a regex that is being used to locate and verify an email address. The code snippet is: 

</br>`\b[a-z0-9#$_-]+@[a-z0-9]+\.[a-z]{2,3}\b/gi`</br>

The beginning and end of the Regex is "\b". That is referred to as the word boundaries. It states that the expression needs to be matched as a stand-alone word. 
The first group (being "[a-z0-9#$_-]+") matches up any upper or lower case letter, number, or the characters #$_-. The "-" used between the "a" and "z" provides the requirement of any letter between those two (the whole alphabet). 0-9 is the same, only for numbers. The "+" sign after the closing bracket means that any of the characters before it can occur one time or more than one. 
Next is the "@" sign. It is always included in emails. After that is the "\." which is the dot before the extension (com).
The last part is the "[a-z]{2,3}" which houses the extension. The first part "[a-z]" is simply the same as earlier, indicating the characters within the range of "A" to "Z". The second part "{2-3}" is defining the minimum and maximum length for the extension (edu).

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)

### Anchors

The "\b" from earlier (the word boundaries) is called an anchor. By using it at the beginning and end, we are using a "whole word" search. An example would be "\b123456\b". Using this, "123456" would match but not "1234567". Other anchors include "^" and "$". "^K" will match a string that starts with "^K" and "K$" will match a string that ends with "K$".

### Quantifiers

A quantifier basically repeats the previous item 0, 1, or more times. The "+" sign is a quantifier. 

### Character Classes

Character classes refer to the characters in between square brackets ("[a-z]"). You can also match specific characters, for example "[katy]" would match k,a,t, or y. 

### Flags

An example of a flag would be the "i" at the end of our example. It basically enables us to match upper and lowercase letters at the same time, without having to type something like "\b[a-zA-Z0-9#$_-]+@[a-zA-Z0-9]+\.[a-zA-Z]{2,3}\b/i". Another example would be the "g" flag. It provides a global search for the Regex definition matches.

### Bracket Expressions

Brackets ("[]") define the character class. Any character placed inside will produce a match to the Regex pattern. 

### Greedy and Lazy Match

A greedy quantifier matches as many items as possible (for example "+"), while a lazy match will attempt to match a Regex pattern once.

### Boundaries

An example of a boundary would be the "\b" from earlier. It indicates that a match will only occur if the string is matched in isolation (is the whole word). 

## Author

My name is Katy Thompson and I am a student in a full stack web development bootcamp. My Github is: [katycaroline](https://github.com/katycaroline)