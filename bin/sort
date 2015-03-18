#!/usr/bin/python
# Alphabetical sort.
# Reads a file with value separated by new lines,
# and output an alphabetical sort list without duplicates.
# author: Nicola Pietroluongo <nik.longstone@gmail.com>

import sys

def main(arg):
    print 'Open Data Sample file check v0.0.1 by Nicola Pietroluongo'
    if (len(arg) > 0):
        alphabeticalSort(arg[0])
    else:
        print 'You must provide a filename'

def alphabeticalSort(filename):
    with open (filename, 'r') as f:
        values = set(value.rstrip ('\r\n') for value in f)
    for value in sorted(values):
        print value

if __name__ == "__main__":
   main(sys.argv[1:])
