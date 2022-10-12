# FLEE
This is a modification of Eugene Ciloci's Fast Lightweight Expression Evaluator to add fixes and functionality for use in LightGuide, Inc. software.

Overall, it provides a few differences from the original, with some java conventions, and other changes more specific to LGS.

## New features:
* Added $ as an acceptable starting character for variable names
* Added && as an alias for AND
* Added || as an alias for OR
* Added : as an acceptable non-starting character for variable names
* Added ! as an alias for NOT
* Added left and right double quotes as aliases for normal double quotes

## Bug fixes:
* Fixed problem with if(,,) expressions not working if a parameter was an expression with too many elements

## Original readme:
```
Flee - Fast Lightweight Expression Evaluator
-------------

Version: 0.9.26.0
Release Date: June 17, 2009
Author: Eugene Ciloci

What is it?
-----------
A .NET library that allows you to parse, compile, and evaluate expressions.  Its main distinguishing feature is that it uses a custom compiler to convert expressions to IL and then emits them to a dynamic method at runtime.  This ensures that expression evaluation is fast and efficient.

What license does it use?
-------------------------
The library is licensed under the LGPL.

Dependencies
------------
The library uses the excellent grammatica parser generator to handle formula parsing.
It is also licensed under the LGPL and you can get the latest version at: http://grammatica.percederberg.net/
The tests use NUnit.

Additional Information
----------------------
The project is hosted on CodePlex.  You can find the project page at: http://www.codeplex.com/Flee

I hope you find it useful
