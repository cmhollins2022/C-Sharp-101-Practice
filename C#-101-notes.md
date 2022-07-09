# C#-101-notes
### Why C#?
- Very versatile.
- A nice syntax.
- Easy to learn more complex things later.
### Hello World
What is a __console__? Whatever is in the quotations will return to the console.
Strings must be explicitly declared.

```string aFriend = "Tyler";```
```Console.WriteLine($"Hello  + {aFriend}");```

### The Basics of Strings
What is a __string__? A series of characters that can be declared. Stored within an array.
The ```Length``` property shows how long the string is.

The ```Trim```, ```TrimStart``` and ```TrimEnd``` methods remove leading and trailing spaces. (Better Formatting)

The ```Replace``` method searches for a substring (or first parameter) and replaces is it with a second parameter. ```ToUpper``` capatelizes each character in a string, and ```ToLower``` changes a string to all lowercase.

What is a __Boolean__ value? Returns a __True__ or __False__.

The ```contains``` method returns a boolean value, showing if the sub-string is within a string. ```StartsWith``` and ```EndsWith``` returns a boolean depending on the posistion of the string within the given parameter.

### Numbers and Integer Math
An ```int``` type represents an integer. All basic operations are represented through ```+ - * /```. Integer division always produces an integer result.

#### Numbers and Integer Precision
If integer division truncates the result, use the ```%``` to produce the remainder.

 
