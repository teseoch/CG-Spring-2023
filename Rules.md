General Rules
=============


Plagiarism Note and Late Submissions
------------------------------------

Copying code (either from other students or from external sources) is strictly prohibited. We will be using automatic anti-plagiarism tools, and any violation of this rule will lead to expulsion from the class. Late assigments will be graded out of 70%.


Provided Software
-----------------

For this class, you will use the minimal framework provided with each assignment. It compiles on Windows, Linux, and Mac. No special hardware is required for this class as we will not be using the GPU for the assignments.

### Preparing the Build Environment

If you are on windows, follow these [detailed instructions](Windows.md).

The assignments will use CMake as a build system. Before we can begin, you must install CMake on your computer.
I recommend installing it with a package manager instead of the [CMake download page](http://www.cmake.org/download/). E.g. on Debian/Ubuntu: `sudo apt-get install cmake`, with HomeBrew on Mac: `brew install cmake`, and on Windows with [Chocolatey](https://chocolatey.org/): `choco install -y cmake`.

You must install a C++ compiler: `gcc/clang` on Linux, `clang` on Mac, [Visual Studio](https://www.visualstudio.com/) on Windows. If you are looking for an IDE to develop in C++, we recommend [Visual Studio Code](https://code.visualstudio.com) on Mac/Linux, and [Visual Studio](https://www.visualstudio.com/) on Windows.

### Compiling the Sample Projects

We will provide a folder for each assignment with some sample code to get you started. Included in each assignment folder is a CMake build system that should enable you to compile your code easily.
For each assignment, you will need to do the following:

1. Download the assignment code
2. Create a directory called `build` in the assignment directory, e.g.:
   ```
   cd assignment_X; mkdir build
   ```
3. Use CMake to generate the Makefile/project files needed for compilation inside the `build/` directory:
   ```
   cd build; cmake -DCMAKE_BUILD_TYPE=Debug ..
   ```
4. Compile and run the compiled executable by typing:
   ```
   make; ./assignmentX
   ```


What to Hand In
---------------

The delivery of the exercises is done using brightspace. The repository should follow the template provided in the starter code, and it must contain:

- The source code, together with any changed CMake project files, but excluding all compiled binaries/libraries. Specifically, do not include the `build/` directory. The code must successfully compile on your operating system of choice: code that does not compile will not be awarded any point, even if it contains a partial implementation of the solution.


Note: It will not be necessary to use additional external software for your assignments. If you find that you need to use additional binaries / external libraries other than those provided by us, please first get approval by sending a message on teams.

Grading
-------

Your submission will be graded according to the quality of your image results, and the correctness of the implemented algorithms. The submitted code must reproduce exactly the images included in your readme.
