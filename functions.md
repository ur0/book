# Functions

When you're writing a slightly larger program, you'll probably not want to write all your code in the `main` function - if you do, things will start getting out of hand soon. This is why break our programs into several `function`s.

## Declaring functions

Here's how you declare a function.

`return-type function_name(type_a arg1, type_b arg2)`

Here, the function returns a value of type `return-type` and takes two arguments `a1` and `a2` of types `type_a` and `type_b` respectively.

For example, here's a function that squares a floating-point number and returns it.

```cpp
float square(float num) {
  return num * num;
}
```

## Calling functions

Calling a function is trivial. Say, using the function above, you wanted to know the square of 6.37. This is how you'd do it.
```
float square_of_6_37 = square(6.37);
```
Now, `square_of_6_37` contains the floating-point value `40.5769`.

## Prototyping functions

Here's our program that prints the square of 6.37.

```cpp
#include <iostream>

using namespace std;

float square(float num);

int main() {
        float square_of_6_37 = square(6.37);
        cout << square_of_6_37 << endl;
}

float square(float num) {
        return num * num;
}
```

There's one line that peeks out here - `float square(float num);`, just after the `using namespace std;`. This line is called the prototype of the `square()` function.
When you're calling the `square()` function, the compiler needs to know the types of the arguments, the number of arguments and the function's return type in order to check the program. When you're prototyping the function, you're giving the compiler all these details beforehand.

You could skip prototyping altogether by defining the function before its calling function (i.e., before `main` here), but this is not recommended. Here's how that'd look like.

```cpp
#include <iostream>

using namespace std;

float square(float num) {
        return num * num;
}

int main() {
        float square_of_6_37 = square(6.37);
        cout << square_of_6_37 << endl;
}
```

One last thing - when you're prototyping a function, you don't need to specify variable names in the prototype. For example, this is a completely valid prototype for our `square()` function.

`float square(float);`

And so is this.

`float square(float asdfgh);`

## More examples

Here are some extra self-explanatory examples (prototypes not included).

```cpp
void just_say_hi() {
  cout << "hi" << endl;
}

int return_one() {
  return 1;
}

void echo_user_input() {
  char userInput[100]; // Create an array of characters
  cin >> userInput;
  cout << userInput << endl;
}
```
