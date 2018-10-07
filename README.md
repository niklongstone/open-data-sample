## Open Data Sample

The Open Data Sample project wants to provide various sample data in an organized way.
The project includes several text/plain files with data in many languages.
The project follows some specification standards to assure the overall quality.

#### Standards:
 - The file name must be lowercase;
 - the file must be a plain text file with .txt extension;
 - every row in the file must be separated by new line;
 - the file cannot contain a blank line inside;
 - the folder's name must respect the [RFC 4647](http://www.rfc-editor.org/rfc/rfc4647.txt) and [RFC 5646](http://www.rfc-editor.org/rfc/rfc5646.txt) specification with the following notation: 
  - `language-region` 
   
 ([language subtag registry](http://www.iana.org/assignments/language-subtag-registry/language-subtag-registry))

#### Licence:
It's released under the [Open Data Commons Open Database License v1.0](http://opendatacommons.org/licenses/odbl/1.0/)
#### Contribution:
Contributions are very welcome but, there are some rules:

1. Don't submit data which can be easily created by most of the programming languages (i.e. day of the week, numbers, dates, ...).
2. Make one pull request for data type. For instance, if you want to add cities and animals please make 2 pull requests.
3. Keep one word per row.
4. Valid character are letters of the alphabet and new lines. 
5. Don't use synonyms or words which are almost equivalent (i.e. cat, kitten).
6. Submit as much data as you can. A submissions with less than 20 rows could be declined. 
7. Avoid the use of headers in the files. For instance, the first row of a city file cannot be "cities".

The project has some tools to simplify the file creation:
 - check (bin/check dataFolder) validates the standard rules.
 - sort (bin/sort filename.txt) outputs an alphabetically sorted list without duplications.

[![Travis Ci](https://travis-ci.org/niklongstone/open-data-sample.svg?branch=master)](https://travis-ci.org/niklongstone/open-data-sample) 
