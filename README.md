# REGULAR EXPRESSIONS 101

## NOTATION CONVENTIONS AND MODES

### Regular expressions
- /abc/
- As in: g/re/p
- Use without forward slashes

### Text string
- "abc"
- Use without quotes

### Modes
- Standard: /re/
- Global: /re/g
- Case-insensitive: /re/i
- Multiline: /re/m
- Dot-matches-all: /re/s

## LITERAL CHARACTERS

### Strings
- /car/ matches "car"
- /car/ matches the first three letters of "carnival"
- Similar to searching in a word processor
- Simplest match there is

### Case-sensitive (by default)

### Standard (non-global) matching
- Earliest (leftmost) match is always preferred

## METACHARACTERS

### Characters with special meaning
- Like mathematical operators
- Transform literal characters into powerful expressions

### Only a few metacharacters to learn
- \ . * + - {} [] ^ $ | ? () : ! =

### Can have more than one meaning
- Depends on how it is used in context

### Variation between regex engines

## THE WILDCARD METACHARACTER

### Matches any one character except newline
- Original Unix regex tools were line-based
- /h.t/ matches "hat", "hot", and "hit", but no "heat"

### Broadest match possible
### Most common metacharacter
### Most common mistake
- /9.00/ matches "9.00", "9500", and "9-00"

    The challenge of regular expressions is both matching what you want and only what you want.

## ESCAPING METACHARACTERS
    \ = Escape the next character

### Allows use of metacharacters as literal characters
- Match a period with \.
* /9\.00/ matches "9.00", but not "9500" or "9-00"
- Match a backslash by escaping a backslash(\\)
### Only for metacharacters
- Literal characters should never be escaped, gives them meaning.

### Quotation marks are note metacharacters, do not need to be escaped.

## OTHER SPECIAL CHARACTERS

### Spaces

### Tabs
- \t

### Line returns
- \r, \n, \r\n

### Non-printable characters
- bell(\a), escape(\e), form feed(\f), vertical tab(\v)

### ASCII or ANSI codes
- Codes that control appearance of a text terminal
- 0xA9 = \xA9
