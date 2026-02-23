# CS-210 Project Three – Corner Grocer Item Tracker

## Project Summary
This program analyzes a grocery store's daily purchase log to determine 
how frequently each item is bought. It reads a plain-text input file, 
tallies item frequencies using a C++ map, and presents results through 
a menu-driven console interface. Users can search for a specific item, 
view a full frequency list, or view a text-based histogram. A backup 
data file (frequency.dat) is written automatically on startup.

## What I Did Well
I structured the program cleanly around a single class with clear 
public and private separation. Using std::map made the data naturally 
sorted and easy to iterate, and I kept the interface logic fully 
separated from the data logic.

## Areas for Enhancement
The histogram could be improved with a GUI or color-coded output for 
readability. File paths could be made configurable via command-line 
arguments rather than hardcoded constants, which would make the program 
more flexible. Adding unit tests for the GroceryTracker class methods 
would improve reliability and make future changes safer.

## Most Challenging Part
The most challenging aspect was handling edge cases in user input — 
ensuring the menu loop couldn't be broken by non-numeric or 
out-of-range input. I solved this using cin.clear() and cin.ignore() 
inside a validation loop, which I researched through cppreference.com 
and the course zyBooks readings.

## Transferable Skills
Working with file I/O, maps, and class design are skills that apply 
directly to future coursework and real-world development. The pattern 
of separating a data class from a UI loop is something I'll use in 
virtually every project going forward.

## Maintainability and Readability
I used consistent naming conventions, in-line comments on every logical 
block, and kept all magic strings as named constants. The class 
encapsulates all data operations so future changes to the data 
structure wouldn't require touching the menu or display code.
