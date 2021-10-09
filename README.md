# Indexer
Indexer is a Python script that generates an .html index of files within a chosen directory. This script generates an .html index of files within a directory (recursive is OFF by default). Start from current dir or from folder passed as first positional argument. Optionally filter by file types with --filter "*.py".

## Pre-requisites:
This project requires you to have Python > 3.x.x installed on your system. **Ideally use current build of Python 3.9 (significantly faster processing!)**

## Usage
***python3 indexer.py /top_dir***

## positional arguments:
⚙ *top_dir*: top folder from which to start generating indexes, use current folder if not specified

## optional arguments:

*⚙ -h, --help: show this help message and exit
* ⚙ -f, --filter: only include files matching glob
* ⚙ -o filename, --output-file filename: Custom output file, by default "index.html"
* ⚙ -r, --recursive*: recursively process nested dirs (FALSE by default)
* ⚙ -v --verbose*: verbosely list every processed file ***WARNING: can take longer time with complex file tree structures on slow terminals.*** 

## Features:

⚙️ Custom icons (if supported by OS)  
⚙️ File Size & Modified Time display 
⚙️ Create custom output file (by default *index.html* is generated
