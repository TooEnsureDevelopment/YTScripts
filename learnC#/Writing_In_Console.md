
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

| **PROBLEM** | **Description** |
| :---: | :--- |
| Multiple name references | Should never have to repeat (DRY CODE) |


**Storing Data**

| **SOLUTION** | **Description** |
| :---: | :--- |
| Variable | Ability to store reusable data (Value) |
| Data Type | Always *specify* the data of *every value and expression* |
| String Interpolation | More readability less ignoring ```+``` *concatenating* |

Create ```name``` variable with type ```string``` equal to ```(Cavis A.)``` to replace repeated name referencing in console.

Then us ```$"{string interpolation}"``` as a substitute for ```+``` concatenating.

```ruby
string myName = "Tech SaVo";   # store my name as string

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