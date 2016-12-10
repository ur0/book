# Getting Started

Before we get up and running, we'll have to know about and install a magical program called a compiler.

## What's a Compiler?

Computers don't directly understand C++. They need a translator, _a compiler_ to turn C++ into a language they understand \(called a binary\). If you want to write your own programs, you will need to install one on your PC. Fortunately for us, there are loads of free compilers out there. They might differ slightly in their specifications, but they do the same thing.

## Installing a compiler

Instructions here differ for each OS. If you're running Windows or some Linux distro, I've got you covered.

### Windows

Code::Blocks is a free and simplistic IDE \(Integrated Development Environment, i.e. a super-powerful text editor\) with an inbuilt compiler. You can download it [here](http://www.codeblocks.org/downloads). Once it downloads, run the downloaded file to install it.

### Linux

You've got two options. If you're comfy with a terminal, you should install and use g++. If the command line freaks you out for whatever reason, you should use CodeBlocks instead \(see the Windows instructions for the download link\).

#### g++

If you're using Debian or Ubuntu, you can install `g++ by running sudo apt-get install g++. That's it.      
To compile a program, you'll run g++ path/to/program.cpp to compile and link the executable, and ./a.out in your current directory to execute it.`

### Mac OS X

You'll too can either install XCode to get the compiler toolchain, or get CodeBlocks \(I highly recommend CodeBlocks becuase installing XCode takes me forever\).

