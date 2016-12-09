# Your First Program

Time to fire up your newly installed IDEs and get our first program running.

## Hello, World!

```cpp
#include <iostream>

using namespace std;

int main() {
    cout << "Hello, World!" << endl;
    return 0;
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
    std::cout << "Hello, World!" << std::endl;
    return 0;
}
```

Notice the two `stds there? Our line above saves us from typing std:: before everything we're taking from iostream. To elaborate on that, it includes the contents of the std namespace (bunch of functions and other things provided to you by the language, stored in files like iostream) into the program so that we don't have to specify it explicitly.`

```cpp
int main() {
```

This line declares a `function. `Functions in programming languages are similar to mathematical functions. They may or may not take parameters, and may or may not produce \(return\) output. When we say int main\(\), we're defining a function named main which takes no parameters \(called arguments\) and returns an integer. The brace following those parantheses encloses the contents of the function. It also has a matching brace \(}\) at the last line, which indicates the end of our function.

