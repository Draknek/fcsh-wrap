MOTIVATION
==========

Compiling Flash applications from the command line using mxmlc is slow. The fcsh tool (also in the Flex SDK) keeps everything in memory for much faster compile times, but you need to keep it running and the shell is rubbish.

This script is a wrapper for fcsh to give it a better user interface and to allow you to run it from make. It runs as a daemon process which manages a fcsh process.


USAGE
=====

1. Download the fcsh-wrap script from http://github.com/Draknek/fcsh-wrap/raw/master/fcsh-wrap
2. Edit the file to point to your copy of fcsh (if it's not in your $PATH)
3. Run fcsh-wrap instead of mxmlc, with all the same arguments.


REQUIREMENTS
============

* Python
* The Flex SDK


KNOWN ISSUES
============

* Output goes to the terminal that you start it running on, even if you’ve closed that window.
* Almost certainly won’t work under Windows, but if you’re running Windows you should probably be using FlashDevelop anyway.
* Leaves .FW.[MD5SUM] files in the working directory.


ACKNOWLEDGEMENTS
================

Based heavily on this original code but with some bugfixes and improvements:
http://www.nabble.com/fcsh-wrapper-to-make-fcsh-work-with-make-td12375081.html



