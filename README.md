# Indexer
Indexer is a Python script that generates an .html index of files within a selected directory. This script generates an .html index of files within a directory (recursive is OFF by default). Start from current dir or from folder passed as first positional argument. Optionally filter by file types with --filter "*.py".

## Prerequisites:
* This script requires you to have **[Python > 3.x.x](https://www.python.org/downloads/)** installed on your system. 
* Ideally use the current build of **[Python 3.10](https://www.python.org/downloads/release/python-3100/)** (significantly faster processing!)

## Usage
*python3 indexer.py /top_dir*

## Positional arguments:
* **top_dir**: top folder from which to start generating indexes, use current folder if not specified

## Optional arguments:
* **-h, --help**: show this help message and exit.
* ***-f, --filter***: only include files matching glob. (EX: indexer.py --filter '**/*.jpg')
* ***-o filename, --output-file filename***: Custom output file, by default "index.html"
* ***-r, --recursive***: recursively process nested dirs (FALSE by default).
* ***-v, --verbose***: verbosely list every processed file. *WARNING: will take longer time with complex file tree structures on slow terminals.*

## Features:
* Custom icons (if supported by OS)  
* File Size & Modified Time display 
* Create custom output file (by default *index.html* is generated
* Ability to match specified parameters using [*glob*](https://docs.python.org/3/library/glob.html) ('**/*.jpg' '**/*.'
