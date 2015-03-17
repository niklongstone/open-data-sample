The Open Data Sample project, wants to provide several sample data in an organized way.  
It's composed by several text/plain files with new line separated data in different languages.  
The project follows some specification standards to assure the overall quality. 

####Standards:
 - The file name must be lowercase;
 - the file must be a plain text file with .txt extension;
 - every lines in the file must be separated by new line;
 - the file cannot contain a blank line inside;
 - the folder's name must respect the [RFC 4647](http://www.rfc-editor.org/rfc/rfc4647.txt) and [RFC 5646](http://www.rfc-editor.org/rfc/rfc5646.txt) specification with the following notation: 
  - languange-region 
   
 ([language subtag registry](http://www.iana.org/assignments/language-subtag-registry/language-subtag-registry))

####Licence:
It's released under the [Open Data Commons Open Database License v1.0](http://opendatacommons.org/licenses/odbl/1.0/)
####Contribution:
Contributions are very welcome.  
The project has some tools for simplify the file creation:
 - check (bin/check.py dataFolder) it validates the standard rules.
 - sort (bin/sort.py filename.txt) it outputs an alphabetically sorted list without duplications.

[![Travis Ci](https://travis-ci.org/niklongstone/open-data-sample.svg?branch=master)](https://travis-ci.org/niklongstone/open-data-sample) 
