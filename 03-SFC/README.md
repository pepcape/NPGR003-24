# Task 03-SFC
Your task is to implement several **Space Filling Curves** and render them into vector
SVG graphics.

Examples of curves can be found, for example, in Wikipedia under
[Space-filling curve](https://en.wikipedia.org/wiki/Space-filling_curve).
Peano, Hilbert, or Dragon curves are examples of curves that either fill the plane
directly or can be used to construct a plane using tessellation.

However, in our problem we do not have to limit ourselves to SFC curves, we will
also accept other fractal curves, you can choose. To successfully complete the task,
you will need to implement at least two different curves (built on different
principles, not variants of the same approach). You will get extra points for
additional unique curves - see below.

# Task
The pilot project includes a C# .NET 8 command-line program that implements
a few simple line parameters and writes the output to the required SVG text file.
We tried to show that no special libraries are needed to write SVG format, but
you can feel free to use other libraries. [SVG.NET](https://github.com/svg-net/SVG)
is one example.

To get familiar with the syntax and semantics of SVG, we recommend this website:
[w3schools - SVG Tutorial](https://www.w3schools.com/graphics/svg_intro.asp).

# Command line arguments
**Mandatory arguments** (you must implement them)
* `-o <filename>` - output SVG file
* `-w <number>` - width of the output rectangular window
* `-h <number>` - height of the output rectangular window
* `-c <curve>` - curve type (can be numeric or string)
* `-d <number>` - "recursion depth" (number of divisions when using a recursive definition)

**Optional arguments** (optional functionality)
* curve drawingstyles
  - color
  - line thickness
  - possible dynamic style (thinning, color gradients)
* fractal curve definition parameters - depends on the curve type

Don't forget to describe all arguments in the **documentation**!

# Output
If all goes well, you should save the SVG file with the required parameters
to disk. Use your web browser to view it.

If the input arguments are not OK, don't draw anything, just print a
clear error message to the console.

# Launch date
**Thursday 24 October 2024**
(Don't work on the solution before this date)

# Deadline
See the shared [point table](https://docs.google.com/spreadsheets/d/11OnE4a-b27eOJ00pfbsYOk7uSdr0hzKrELs_vFG3a_Q/edit?usp=sharing).

# Credit points
**Basic solution: 8 points**
* must not crash under any circumstances
* you must implement all mandatory arguments (`-o`, `-w`, `-h`, `-c`, `-d`)
* at least two different fractal curves, at least one must be able
  to fill the plane by itself (SFC curve)
* you must accept any reasonable image (window) size, if your drawing needs
  a specific aspect ratio, enclose it in a smaller rectangle. Do not distort
  the scales on the coordinate axes!

**Bonus points: up to 7 additional points**
* interesting graphic design (color, line thickness, gradients)
* more curve types (beyond the mandatory number of 2)
* don't limit your creativity (as long as the compulsory part is included) - you can
  try different combinations of curves, etc.

## Use of AI assistant
Using an AI assistant is recommended! But you have to be critical and
test all its suggestions thoroughly. In particular, test singular cases
(trivial recursion depth, limiting window dimensions or aspect ratios).