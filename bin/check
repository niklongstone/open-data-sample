#!/usr/bin/python
# Data file checker 
# Open data sample project 
# author: Nicola Pietroluongo <nik.longstone@gmail.com>

import os
import sys
import string

testReport = []
testResult = True

def main(arg):
    print 'Open Data Sample file check v0.0.1 by Nicola Pietroluongo'
    if (len(arg) > 0):
        checkDataFiles(arg[0])
    else:
        testReport.append('You need to provide a folder to check es: check.py folder')
    printTestReport()
    returnResult()

def checkDataFiles(dataFolder):
    if os.path.exists(dataFolder):
        for root, subFolders, files in os.walk(dataFolder):
            for file in files:
                filePath = os.path.join(root, file)
                checkFile(filePath, file)
    else:
        testReport.append('The directoty "{}" does not exist'.format(dataFolder))
                
def checkFile(filePath, file):
    if (hasUppercase(file)):
        testReport.append('The file name "{}" cannot contain uppercase letters'.format(filePath))
    if (hasBlankLines(filePath)):
        testReport.append('The file "{}" cannot contain blank lines'.format(filePath))

def hasUppercase(fileName):
    return (len(set(string.ascii_uppercase).intersection(fileName)) > 0)

def hasBlankLines(file):
    with open(file, 'r') as file:
        for line in file:
            if line in ['\n', '\r\n']:
                print line
                return True
            else:
                return False

def printTestReport():
    if len(testReport)> 0:
        testResult = False
        print 'TEST FAILURES:'
        for report in testReport:
            print report
    else:
        print 'TEST SUCCESS'

def returnResult():
    return testResult

if __name__ == "__main__":
   main(sys.argv[1:])

