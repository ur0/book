# Variables

When you're programming, you'll often want to store data like something your user entered, a random number or pretty much everything else. Variables in C++ \(and pretty much everywhere else\) are used to store data, and they're something we need to figure out before we write more complicated programs.

## Variable Types

Variables have a _type_ corresponding to the type of the data they hold. If you were to store an integer like 3, you'd use a variable of type _int_ \(short for integer\). If you wanted to store the value of Pi, 3.1415, you'd use a _float_ \(short for a floating-point number\). You also have the _double_ type, which is a double precision floating point type \(it is more precise than _float_, the exact precision depends on your compiler and environment\).

Similarly, if you wanted to store a single letter, say 'C', you'd use a _char_ type. If you wanted to store just a boolean - a simple _true_ or _false_, you'd use the _bool_ type.

Here's a list of the fundamental types in C++ \(you'll rarely encounter the last two, they're included just for completeness' sake\).

| Type | Description |
| :--- | :--- |
| _bool_ | Stores either _true \_or \_false._ |
| _char_ | Stores a single character and occupies a single byte. |
| _int_ | Stores an integer. Usually, this can store values from -127 to 127. |
| _float_ | Stores a decimal number with single precision. |
| _double_ | Stores a decimal number with double precision. |
| _void_ | \_void \_denotes the absence of type - a void variable has no type. |
| _wchar\_t_ | A wide-character type. |

## Declaring Variables

Before you use a variable, you need to _declare_ it, i.e., you need to tell the compiler the type of the variable and its value. Here's a variable declaration.

```
int my_integer = 123;
```

In the line above, we're declaring an \_integer, \_and assigning it a value of 123.

Similarly,

```
float pi = 3.1415;
char the_letter_z = 'z';
double really_precise_physics_result_thingy = 12.329371782;
```

All the lines above declare a variable, preceeded by its type and also assign it a value.

You can declare a variable without assigning it a value too, as long as you use it only after assigning it a value.

```
int independence; // We're just declaring a variable named independance here.
```

You could assign this variable a value later, somewhat like this.

```
independence = 42;
```

Now you could use independence however you like it.

```
cout << "Independence is: " << independence << endl; // Will print "Independence is 42" to the screen.
independence = independence - 13; // independence is now equal to 29
cout << "Independence is now: " << independence << endl; // Will print "Independence is now 29" to the screen.
```



