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

### Numbers and Integer Precision
If integer division truncates the result, use the ```%``` to produce the remainder. ```MaxValue``` and ```MinValue``` show the limits of integers. If you go above the maximum, or below the minimum, you will __overflow__ or __underflow__.

A ```Double``` numeric type represents a double-precision floating point number. Double precision numbers have twice the number of binary digits as single-precision.

### Numbers and Decimals
The ```decimal``` type has a smaller range but greater precision than ```double```. There is also ```long```'s and ```short```'s that assist with being precise. An ```int``` will be enough in most cases though.

### Branches (if)
```if``` this, then something will happen. This conditional is a form of a ```bool```, which can also be explicitly declared to determine if something is ```true``` or ```false```. If one side of the answer is true ```&&``` the next side of the answer is true, then the console will return True. However, if one side of the answer is true ```||``` (or) the other side of the answer is true, then the console will also return True.

### Hello world explained
```using``` includes any libraries you use, including "System", for the console log. ```namespace```'s are used to group and organize code. Group multuple different classes together to keep everything organized. ```Class``` declared a class, and ```static void Main(string[] args)``` is your first (or main) method.

### What are loops?
Loops help us to repeat statements. ```while``` something is ```true```, it will repeat. You can also ```do``` something first, then check the conditional after using ```while```. Incriment using some variable```++```.

You can use a ```for``` loop in oder to make varient types of conditional statements:
The first part is the __for initializer__: ```int counter = 0;``` declares that ```counter``` is the loop variable, and sets its initial value to ```0```.

The middle part is the __for condition__: ```counter < 10``` declares that this for loop continues to execute as long as the value of ```counter``` is less than 10.

The final part is the for iterator: ```counter++``` specifies how to modify the loop variable after executing the block following the for statement. Here, it specifies that ```counter``` should be incremented by 1 each time the block executes.
```
for(int counter = 0; counter < 10; counter++)
{
  Console.WriteLine($"Hello World! The counter is {counter}");
}
```

### Combining Branches and Loops
Proper __scoping__ allows for variables to be declared and assigned in the correct order.
```
int sum = 0;
for(int i = 1; i <= 20; i++)

{
    if(i % 3 == 0)
    {
        sum = sum + i;
    }
}
Console.WriteLine($"The sum is {sum}");
```

### Arrays, List, and Collections
```var``` is used when you are not sure what your variable will be. A ```List``` must be explicitly declared along with the type that will be contained within the list. Lists can be a  ```list<of>``` any types. 
```
var names = new List<string> { "<name>", "Ana", "Felipe" };
foreach (var name in names)
{
  Console.WriteLine($"Hello {name.ToUpper()}!");
}
```
Arrays are usually '0' based, starting at the ```[0]```'th position.

### Sort, Search, and Index Lists
The ```IndexOf``` method searches for the given parameter value and returns the index. The ```Sort``` method sorts the items within a list normally. Each character of a string (or ```char```) have numerical values. So, when they are sorted, the computer knows to sort them alphabetically.

### Debugging
A __Break point__ (red dot) will pause the code at a specific point, and allow for further analysis.

### Object Oriented Programming - Objects and Classes
With Object Oriented Programming (OOP), we can classify objects with various attributes. We can make a ```class```, along with ```public``` or ```private``` attributes. Again, it is necessary to explicitly declare the variable type.

We can make a class, and it is good practice to make one file per class. *"If the code reads like a haiku, then you've done it correctly."*
