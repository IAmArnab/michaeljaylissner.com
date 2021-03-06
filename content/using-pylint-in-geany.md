Title: Using Pylint in Geany
Date: 2010-08-11T12:07:23
Tags: Python, pylint, geany
Category: Tech

<a href="http://www.logilab.org/857">Pylint</a> is a tool that tells you 
when your Python code is broken or when it has coding problems. As a newish 
Python coder, using it has taught me a lot about conventions, 
and has helped to make my code significantly cleaner. Enabling it in my IDE,
 <a href="http://www.geany.org/">Geany</a>, makes it so that using it is 
 just another part of my development workflow. 

Enabling Pylint in Geany is easy. Simply open Geany, and create a new build 
command that uses `pylint -r no "%f"` as the command, and `(W|E|F):([0-9]+):
(.*)` as the error regular expression. After you've done this, 
using this build command instead of saving your work will run Pylint on your
 current file, showing you warnings, errors and fatal errors in red.
