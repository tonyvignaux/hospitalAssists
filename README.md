# hospitalAssists
The program to graph the weekly numbers of assists in Wellington CCDHB hospitals

It was first written as  Python program and then turned into a Jupyter system.
This is transferring my Jupyter version to GitHub

===========
README
===========

..    Current program version 2.15
      gav 2016.01.08

``weeklyplot.py`` is a Python program to graph the weekly count of the
number of Assistances recorded by volunteer Guides.

Each day the numbers are recorded in the log book. The counts for the
two shifts (Morning and Afternoon) are recorded separately and then
summed for the day. Experience indicates that this data should be
checked independently.

Each week the total number of assistances in the prevous week is
copied to a spreadsheet, one for Wellington Regional Hospital and the
other for Keneperu. Each row holds the data for one week and contains
the date (of the Monday of the week) and the number of assists
recorded in that week. Graphs could also be produced from these
spreadsheets.

So that I can use an independent ``python`` program, the two
spreadsheets are then ``exported`` as ``csv`` (comma separated
variable) files by the spreadsheet program. These are pure text
files of (date,count) pairs to be read by the program. A typical row
is: ``28/09/2009,444,``. The two files are ``weekly.csv`` and
``kene.csv``.

The two files are read by the main Python plotting program,
``weeklyplot.py`` to display a graph. This can (on a Mac, at least) be
either copied or saved to disk.

