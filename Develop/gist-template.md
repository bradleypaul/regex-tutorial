# URL Regex Tutorial



## Summary
This regex is used to find all valid urls in a list of urls.
```javascript
/^(https?:\/\/)?([\da-z\.-]+)\.(c{2,6})([\/\w \.-]*)*\/?$/gim
```

## Table of Contents

- [Anchors](#anchors)
- [Character Classes](#character-classes)
- [Bracket Expressions](#bracket-expressions)
- [Quantifiers](#quantifiers)
- [Flags](#flags)
- [Boundaries](#boundaries)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

### Anchors

```
^http   matches any string that starts with http
html$   matches a string that ends with html
^http$  exact string match (starts and ends with http)
http    matches any string that has the text http in it
```

### Character Classes

```
\d  matches a single digit 0-9
\w  matches a word character a-z, A-Z and _
.   matches any character -> Try it!
```

### Bracket Expressions

```
[\da-z\.-] matches a string with one character between 0-9, a-z, . or -
[\/\w \.-] matches a string with one character \, \w, . and -
```

### Quantifiers

```
\w*           matches a string that has ab followed by zero or more word characters
[\da-z\.-]+   matches a string that has one or more [\da-z\.-] match
https?        matches a string that has http followed by zero or one s
http{2}       matches a string that has htt followed by 2 p
http{2,}      matches a string that has htt followed by 2 or more p
[a-z\.]{2,6}  matches a string that has any character a-z or .  between 2 up to 5 times

```

### Flags

```
i   case insensitvity on
g   global: find all matches
m   multi-line: $ and ^ match line beginnings and ends
```

### Boundaries
```
\bhttp\b          performs a "whole words only" search for http
\Bhttp\B          matches only if the pattern is fully surrounded by word characters
```

## Author
[https://github.com/bradleypaul](https://github.com/bradleypaul)
Full Stack Developer with 5+ years of experience of programming and teaching looking for opportunities using JavaScript and Python. Based primarily in the Austin area but open to remote.
