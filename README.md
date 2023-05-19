# Project 3 - Loops

You will write a program that outputs a downwards facing arrow composed of a
rectangle and a right triangle. Arrow dimensions are defined by user specified
arrow base height, arrow base width, and arrow head width.

## Important Links

- Review the [grading rubric](https://shanepanter.com/cs452/grading-rubric.html)

## Objectives

- Use cin to read data from the user
- Use cout to output to the standard output stream
- Use if/else statements
- Use loops

## Task 1 - Write the program

Step 1. Input the arrow base height (int) and width (int). Draw a
rectangle using asterisks (height x width). Hint: use a nested loop in which the
inner loop draws one row of *s, and the outer loop iterates a number of times
equal to the height. Submit for grading to confirm two tests pass.

```bash
Ex: If input is:

6 4
Sample output is:

****
****
****
****
****
****
```

Step 2. Input the arrow head width and draw a right triangle. Hint: use
a nested loop. Submit for grading to confirm four tests pass.

```bash
Ex: If input is:

4 3 4
Sample output is:

***
***
***
***
****
***
**
*
```

Step 3. Modify the program to only accept an arrow head width that is larger
than the arrow base width. Use a loop to continue inputting the arrow head width
until the value is larger than the arrow base width. Submit for grading to
confirm all tests pass.

```bash
Ex: If input is:

4 3 3 2 4
Sample output is:

***
***
***
***
****
***
**
*
```

## Task 2 - Generate Build Files

There are two scripts in the root directory named `clean.sh` and `release.sh`.
One creates a release build to compile your project and the other will delete
all the temporary files that are created during the build process.

Run the `release.sh` script from the terminal to setup your project. Note
that your output will be slightly different than what is shown below because
cmake configures the build system specific to the system that it is running on.

```bash
shane|(master *%=):solution$ ./release.sh
-- The CXX compiler identification is AppleClang 14.0.3.14030022
-- Detecting CXX compiler ABI info
-- Detecting CXX compiler ABI info - done
-- Check for working CXX compiler: /Library/Developer/CommandLineTools/usr/bin/c++ - skipped
-- Detecting CXX compile features
-- Detecting CXX compile features - done
-- Configuring done
-- Generating done
-- Build files have been written to: ...
```

## Task 3 - Compile your code

After you have run `release.sh` you can `cd` into the build directory to compile
and run the program.

```bash
shane|(master *%=):build$ make
[ 50%] Building CXX object src/CMakeFiles/myprogram.dir/solution.cpp.o
[100%] Linking CXX executable ../myprogram
[100%] Built target myprogram
```

If your code that you wrote in task 1 was correct you should see a executable
named `myprogram` that you can now run to see the output. If your program did
not compile you will need to return to task 1 and fix your code and then return
to this task to compile your code again. You only need to run the `release.sh`
script once if you are recompiling you can skip Task 2 above.

## Task 4 - Complete the Retrospective

Once you have completed all the tasks open the file **Retrospective.md** and
complete each section that has a TODO label.

For the **Experience** section you need to detail your experience with this lab.

- Were there any things that you struggled with?
- Were there any parts of this lab that were unclear or poorly specified?
- Were you able to get the entire project done?

For the **Known issues or Bugs** section you need to detail any issues or bugs
that you have in your code. For example maybe your code crashes randomly and you
couldn't figure out why. If your code doesn't have any issues you can simply
write NONE in this section.

For the **Sources used** section you must detail any sources you used outside of
the textbook or course website. If you write NONE in this section it is assumed
that you didn't use google at all. Be safe CITE!

## Task 5 - Add, Commit, Push your code

Once you are finished you need to make sure that you have pushed all your code
to GitHub for grading! You will not be submitting anything to canvas everything
will be submitted through GitHub as demonstrated in class.
