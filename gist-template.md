# Regular Expressions for Characters

The tutorial will outline how to extract only characters from a variety a data types. The code is executed using JavaScript.

## Summary

The regex will explain the following code snippet.

`/[A-Za-z]/g`

The purpose is to show how to search through data which contains numbers, characters and special characters and return only the alphabet characters from the data.

The example script used to test the regex is below:

const towns = "I li3ve in Bi8rmingha7m tow!@n";
const regexTown = /[A-Za-z]/g;
console.log(towns.match(regexTown));

The expected output is:

IliveinBirminghamtown

Feel free to try other examples and data types.

## Table of Contents

- [Patterns](#patterns)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Bracket Expressions](#bracket-expressions)

## Regex Components

### Patterns

The two forward slashes / identify the pattern enclosed between them as a regular expression. The regular expression in this example is comprised of simple characters which are the full range of the alphabet, `A-Za-z`.

### Character Classes

The character classes identify different types of characters. Simple alphabetic characters `A-Za-z` are used to search and return both uppercase and lowercase character matches only. Any special characters and digits should not return a match to the search criteria, hence be excluded from the output.

This is tested using:

`const towns = "I li3ve in Bi8rmingha7m tow!@n";`

### Flags

The modifier or flag `g` in this example, used at the end of the regex expression, performs a global match to the search criteria. This means all matches to the search criteria will be returned and the search does not stop at the first instance found.

### Bracket Expressions

The brackets `[]` surrounding the pattern, are used to search for a range of characters within the brackets. The range in this example is the alphabet.

## Contributors

Sources viewed to help in the creation of the gist:

https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_expressions#using_the_global_search_flag_with_exec

https://www.w3schools.com/jsref/jsref_obj_regexp.asp

https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_expressions/Character_classes

## Author

If you have any questions about the repo, you can contact me on email: salmy75987@gmail.com

You can also open an issue to contact me or find more of my work at: SALMY001 (https://github.com/SALMY001)
