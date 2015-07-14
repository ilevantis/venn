venn
====

Bash wrapper for simple set operations using sort and uniq

Usage:
------
``venn file1 file2 [option [file3]]``

Options:
--------
-a              Prints lines found in file1 AND NOT in file2.

-b              Prints lines found in file2 AND NOT in file1.

-c              Prints lines found in file1 AND in file2. This is
                the default mode if no option is given.

-d file         Takes a file (file3) as an option argument. All lines present
                in file1 and file2 must be present in file3. Prints lines
                found in file3 NOT found in file1 AND file2.

-e file         Takes a file (file3) as an option argument. Outputs 4 files
                containing the results of modes -a, -b, -c, -d.

-s file         Takes a file (file3) as an option argument. Shows
                the user if the lines in file3 are a superset of lines in file1
                and file2.

-h              Prints a help message.
