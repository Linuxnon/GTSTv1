# Regular Expressions! /regex/

- How do this site know that our input is not email?

# Cont…

● Most filter Validation on any platform done by Regular 
expression/regex/.

● They are patterns that helps to filter so texts,space,tabs & 
symbols.

● Like telegram or other platforms filtering links inside 
group, filtering some bad words.. All are regex.

● Regex is PATTERN!

● Regex are used on linux tools called grep,awk and sed.

## Metacharacters 
● Those are regex pattern symbols for filter.

● They are :

# Dot ( . )

● Used to get All the line except new lines
● Syntax: 

○ This means give me all lines except the new lines

# Caret ( ^ ) - Assertion 

● Used to get line that start with pattern

● Syntax: ^hello

○ This means lines that start with hello

# Dollar sign( $ ) - Assertion 

● Used to get line that ends with some pattern.

● Syntax: hello$

○ That ends with hello

# Plus ( + ) - Quantity 

● Used to get line that have pattern that occurs 1 and more times.

● Syntax: hellos+

○ A text hello that have s at least 1 times and more.

# Asteriks ( * ) - Quantity 

● Used to get line that have pattern that occurs 0 and more times.

● Syntax: hellos*

○ A text hello that have s at least 0 times and more.

# Question mark ( ? ) - Quantity 

● Used to get line that have pattern that occurs 0 and 1 times.

● Syntax: hellos?

○ A text hello that have s at least 0 time or 1 time.

# Curly Bracket ( { min , max} ) - Quantity

● Used to get line that have pattern that occurs min and max times.it is custom.

● Syntax: hellos{1,3}

○ A text hello that have s at least 0 times and more.

# \w 

● Used to get Alphanumeric.

● Syntax: \w

○ All texts except newlines and symbols

# \W 

● Used to get All except Alphanumeric 

● Syntax: \W

○ All texts except newlines and symbols

 # \s 
● Used to get whitespace.

● Syntax: \s

○ All spaces and tabs

# \S 

● Used to get all except whitespace.

● Syntax: \S

○ All spaces and tabs

# \d 

● Used to get Digits/numbers/

● Syntax: \d

○ All spaces and tabs

# \D 

● Used to get all except Digits/numbers/

● Syntax: \D

○ All spaces and tabs

# Pipe ( | ) - OR

● Used to search 2 different things.

● Syntax: a|b

# Escape ( \ ) 

● Used to search symbols that are metacharacters.

● Syntax: \sign

# Square Brackets ( [ ] ) - Custom pattern

● Used to Create your own patterns

● Syntax: [pattern]

## Bash regex

● You can use it on awk, sed, but for today i will show you using grep.

## BASH FOR REGEX

- We can use =~ operator for regex check with if condition statements
