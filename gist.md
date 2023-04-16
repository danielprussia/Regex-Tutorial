# REGEX Tutorial
WELCOME!! This is a Regex Tutorial on the specific regular expression ^[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Za-z]{2,}$
This is a basic regex for setting up Email validation and restrictions
Thank you for Choosing this regex tutorial and i hope it helps!

## Summary
^[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Za-z]{2,}$
This regular expression is commonly used to validate email addresses. It matches any string that follows the general format of an email address.

^ matches the start of the string.

[A-Za-z0-9._%+-]+ matches one or more characters that can be letters (both uppercase and lowercase), digits, or some special characters that are commonly used in email addresses, such as ". _ % + -"

@ matches the @ symbol that separates the local part of the email address from the domain part.

[A-Za-z0-9.-]+ matches one or more characters that can be letters (both uppercase and lowercase), digits, or the . (period) and - (hyphen) symbols that are commonly used in domain names.

\. matches a literal . (period), which separates the second-level domain from the top-level domain.

[A-Za-z]{2,} matches two or more characters that can be letters (both uppercase and lowercase), representing the top-level domain.

$ matches the end of the string.

So, this regular expression would match strings like john.doe@example.com, jane.smith123@hotmail.co.uk, and info@mycompany.com.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)

## Regex Components

^: This symbol matches the start of the string. It ensures that the regular expression will only match if the pattern begins at the start of the string. In this case, it means that the email address must begin at the start of the string.

`[A-Za-z0-9._%+-]+: This is a character class that matches one or more characters that can be letters (both uppercase and lowercase), digits, or some special characters that are commonly used in email addresses, such as . (period), _ (underscore), %, +, and -. 

@: This matches the @ symbol that separates the local part of the email address from the domain part.

[A-Za-z0-9.-]+: This is another character class that matches one or more characters that can be letters (both uppercase and lowercase), digits, or the . (period) and - (hyphen) symbols that are commonly used in domain names.

\.: This matches a literal . (period). It needs to be escaped with a backslash \ because . is a special character in regular expressions that matches any character except a newline.

[A-Za-z]{2,}: This is another character class that matches two or more characters that can be letters (both uppercase and lowercase), representing the top-level domain.

$: This symbol matches the end of the string. It ensures that the regular expression will only match if the pattern ends at the end of the string. In this case, it means that the email address must end at the end of the string.

So, the regular expression as a whole matches any string that follows the general format of an email address.

### Anchors
 The anchors in this regular expression are the ^ and $ symbols.

The ^ symbol is called the "caret" and it matches the start of the string. It ensures that the regular expression will only match if the pattern begins at the start of the string. In this case, the ^ symbol is used at the beginning of the regular expression to ensure that the email address matches from the very beginning of the string.

The $ symbol is called the "dollar" and it matches the end of the string. It ensures that the regular expression will only match if the pattern ends at the end of the string. In this case, the $ symbol is used at the end of the regular expression to ensure that the email address matches all the way to the end of the string.

So, the combination of the ^ and $ symbols anchors the regular expression to match only strings that fully match the pattern of an email address from beginning to end. Without these anchors, the regular expression could match substrings of a larger string that happen to contain the pattern of an email address.

### Quantifiers
There are two quantifiers used in this regular expression:

+: This quantifier matches one or more occurrences of the preceding element. In this case, it is used to match one or more characters from the character classes [A-Za-z0-9._%+-] and [A-Za-z0-9.-].

{2,}: This quantifier matches two or more occurrences of the preceding element. In this case, it is used to match two or more characters from the character class [A-Za-z].

Together, these quantifiers allow the regular expression to match a range of different email addresses with varying lengths of local and domain parts. The + quantifier ensures that the local and domain parts of the email address each contain at least one character, while the {2,} quantifier ensures that the top-level domain contains at least two characters.

### Character Classes
There are three character classes used in this regular expression:

[A-Za-z0-9._%+-]: this class matches any letter uppercase or lowercase, digit, or one of the following special characters: ".  _  % +  - "These characters are commonly used in email addresses.

[A-Za-z0-9.-]: This character class matches any letter uppercase or lowercase, digit, or the period and dash symbol: ".  -" 
[A-Za-z]: This character class matches any letter uppercase or lowercase. It is used to match the top-level domain, which is always composed of one or more letters.

### Grouping and Capturing
The first grouping [A-Za-z0-9._%+-]+ matches one or more characters that are either letters uppercase or lowercase, digits, or the special characters . _ % + or - This group matches the local part of the email address before the "@" symbol.

The second grouping [A-Za-z0-9.-]+ matches one or more characters that are either letters uppercase or lowercase, digits, or the special characters . or - This group matches the domain name of the email address and captures it in a capturing group.

The third grouping [A-Za-z]{2,} matches two or more characters that are either uppercase or lowercase letters. This group matches the top-level domain (TLD) of the email address, such as "com", "net", or "org".
By using a capturing group, the domain name of the email address can be extracted from the match result for further processing or analysis.

### Bracket Expressions
there are three bracket expressions:

[A-Za-z0-9._%+-]: This bracket expression matches any letter uppercase or lowercase, digit, or one of the following special characters: .  _  % +  -

[A-Za-z0-9.-]: This bracket expression matches any letter uppercase or lowercase, digit, or one of the following special characters: . and - 

[A-Za-z]: This bracket expression matches any letter uppercase or lowercase.

### Greedy and Lazy Match
 All quantifiers used are greedy by default. A greedy quantifier will try to match as much of the input string as possible, while still allowing the overall regular expression to match.

For example, in the regular expression ^([A-Za-z0-9._%+-]+)@([A-Za-z0-9.-]+)\.[A-Za-z]{2,}$, the + quantifiers used in both capturing groups are greedy. This means that they will match as many characters as possible that fit the character class, subject to the overall requirement that the entire regular expression must still match the input string.

### Boundaries
 the ^ and $ symbols are also known as boundary markers, which indicate the start and end of the input string.
 The ^ symbol matches the beginning of the input string, and the $ symbol matches the end of the input string,
 Together, these boundary markers ensure that the regular expression matches the entire input string, rather than just a part of it.


## Author

Good evening ladies and gentlemen my name is Daniel Prussia and i am the creator of this Email regex tutorial, i hope this has brought you much enlightenment in the world of tommorow.
Github: github.com/Billthebaker
Portfolio: https://billthebaker.github.io/Portfolio/
