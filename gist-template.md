# Regex Tutorial on Matching an Email

    Regular expressions can be used to find certain patterns of characters within a string. You can also find and replace a character or sequence of characters within a string. They are also frequently used to validate input. This regex matches character information for valid e-mail addresses.

## Summary

    This is the regex code that we will be analyzing today is: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs and Capturing](#grouping-constructs-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [Greedy and Lazy Match](#greedy-and-lazy-match)


## Regex Components

### Anchors

    The anchors used to contain this regular expression are: ^ to start, and $ to finish.

### Quantifiers

    In this example, we used + to communicate there is another sequence to be matched as a greedy quantifier. We also used {2,6} as another greedy quantifier to specify the input should be a minimum of 2 characters to a maximum of 6 characters.

### Grouping Constructs and Capturing

    There are three groups being captured in this example. Group #1 is the username of the e-mail account [a-z0-9_\.-]. The second group captures the domain name or e-mail service being used [\da-z\.-]. Lastly, the third group captures the domain extension (i.e .com or .net) [a-z\.]{2,6}    

### Bracket Expressions

    Much like the groups in this example, there are also 3 bracket expressions. The information in the bracket expressions is opened and closed between brackets like this []. This identifies which information is allowed to be matched.

>Bracket Expression #1: [a-z0-9_\.-] - includes case sensitive characters from a-z, numbers from 0-9 an underscore, periods and hyphens.

>Bracket Expression #2: [\da-z\.-] - includes all digits, case sensitive characters from a-z, periods and hyphens

>Bracket Expression #3: [a-z\.] - includes case sensitive characters from a-z and periods.

### Character Classes

    In this regular expression, the character class /d is used which in Javascript classifies the use of any digit from 0 to 9.

### Greedy and Lazy Match

    In this example we have only used greedy quantifiers + and {}, meaning that it will allow the match to expand as long as it needs to go. If these quantifiers were lazy quantifiers, they would appear as +? or {}?, this will direct the system to make the shortest match.

## Author

My name is Ariel Martinez, and I am getting better as a coder!

Here is my github profile: https://github.com/arielo5
