
# Writing to the console

**Writing**

Printing name to the console

```ruby
static void Main(string[] args)     # Don't worry much here
{       # Start block
    Console.WriteLine("Hello I'm Tech SaVo");   # Prints text to console
    Console.WriteLine(
        "Yesterday, my firend Cavis got into some trouble\n" +
        "Cavis mom is a nice lady but sometimes she can have her limits with Cavis"
        );  # Prints text to console
}       # End block
```

1. Focus mainly on the ```main()``` method (or function).
    - Any code inside block is executed
    
2. ```Console.WriteLine()``` is a command that prints text to the console.
    - Whatever is in between the parentheses will be printed.


**Storing Data**

*PROBLEM*

Decide to enter initial of last name (Cavis A.) rather then just first name (Cavis)

*SOLUTION*

1. Create variable
    - ability to store data and reuse

2. Create Variable Data Type
    - C# is known as a strongly typed language
        - It allows that the programmer *specify* the data of *every value and expression*

3. Use *String Interpolation* ```$"Text {variable}"```
    - more code readability


Create ```name``` variable with type ```string``` equal to ```(Cavis A.)``` to replace repeated name in console.

```ruby
string myName = "Tech SaVo";   # store my name n as string

string friendName = "Cavis A."; # storing friend name as string

static void Main(string[] args)     # Don't worry much here
{       # Start block
    Console.WriteLine($"Hello I'm {myName}");   # Prints text to console
    Console.WriteLine(
        $"Yesterday, my firend {friendName} got into some trouble\n" +
        $"{friendName} mom is a nice lady but sometimes she can have her limits with {friendName}"
        );  # Prints text to console
}       # End block
```