# Your First Program

Time to fire up your newly installed IDEs and get our first program running.

## Hello, World!

```cpp
#include <iostream>

using namespace std;

int main() {
    cout << "Hello, World!" << endl; // Actually print the text
    return 0;
    // That's it
}
```

Confusing, eh? It always is. I mean, there are lots of symbols and words you don't recognize and whatnot. Don't worry, we're gonna come around to it.

### What does this even do?

Great question. This program prints the text, "Hello, World!" to the screen. Agreed, it sure is a lot of work just to print a line of text on the screen, but each of those lines do serve a purpose. Let's look at our program line-by-line.

```
#include <iostream>
```

The line above includes a snippet of code into your program. More specifically, it adds some functions which your computer needs to print text, handle inputs and other input-output related stuff \(hence the name, `iostream).`

```
using namespace std;
```

This line reduces the amount of text you need to type by some extent. Here's a version of our program, without this line.

```cpp
#include <iostream>

int main() {
    std::cout << "Hello, World!" << std::endl;  // Actually print the text
    return 0;
    // That's it
}
```

Notice the two _stds_ there? Our line above saves us from typing std:: before everything we're taking from iostream. To elaborate on that, it includes the contents of the std namespace \(bunch of functions and other things provided to you by the language, stored in files like iostream\) into the program so that we don't have to specify it explicitly.

Also, most lines in C++ \(except lines where we're opening a block, like a function or lines beginning with a \# character\) end with a semicolon.

```cpp
int main() {
```

This line declares a `function.`

Functions in programming languages are similar to mathematical functions. They may or may not take parameters, and may or may not produce \(return\) output. When we say _int main\(\)_, we're defining a function named main which takes no parameters \(called arguments\) and returns an integer. The brace following those parantheses encloses the contents of the function. It also has a matching brace \(_}_\) at the last line, which indicates the end of our function. Here's a special thing about \_main - \_it is the first function that is executed by your computer when you run it.

```cpp
cout << "Hello, World!" << endl; // That's it
```

This line is composed of three different things. _cout_ is a _stream_ in which you insert "Hello, World!" and also insert something called _endl_. Here's the special thing about cout - whatever you insert into it gets printed onto the screen. So, when you insert the text \(which we refer to as a _string_\) into _cout_, the text gets printed onto the screen.

_endl_ has a small story of its own too. When you insert an _endl_ into cout, your computer stops printing text on the current line and switches to a new line.
Also, everything after the `//` is called a comment and is ignored by the compiler.

`return 0;`

This is both the smallest and the most confusing line for new programmers. This returns an _integer _\(remember _int main_?\) with the value of 0. Why does it do that deserves its own special explanation, but remember this - when you write the _main_ function, you should always return a 0 unless your program hit some sort of an error.

You can also get away with not writing this line. If you omit this line, your compiler will assume that you want to return zero.

`// That's it`

The entirety of the line above is a comment and will be ignored. Comments have no significance to the compiler but are useful to let fellow programmers (or sometimes, even yourself) know what's going on.

So that was it, your first program. If you're not thoroughly rattled, keep going. If you are, remember that you're just starting out on a long and entertaining journey, don't sweat it.
