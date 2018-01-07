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