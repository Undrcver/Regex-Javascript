## Regex Javascript Jist
## Regular Expression Constructor
Syntax: new RegExp(pattern[, flags])

Example:

var regexConst = new RegExp('abc');


#Regular Expression Literal
Syntax: /pattern/flags

Example:

var regexLiteral = /abc/;

#Major Example
var regex = /hello/;
var str = 'hello world';
var result = regex.test(str);
console.log(result);
// returns true

#Simple Pattern 
var regex = /hello/;
console.log(regex.test('hello world'));
// true


##Special characters
#Flags:
g — Global search, don’t return after the first match
i — Case-insensitive search

#Simple example for flag use
var regexGlobal = new RegExp('abc','g')
console.log(regexGlobal.test('abc abc'));
// it will match all the occurence of 'abc', so it won't return // after first match.
var regexInsensitive = new RegExp('abc','i')
console.log(regexInsensitive.test('Abc'));
// returns true, because the case of string characters don't matter // in case-insensitive search.

-Luis Alicea
