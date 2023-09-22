[![Python](https://img.shields.io/badge/-Python-464646?style=flat&logo=Python&logoColor=56C0C0&color=008080)](https://www.python.org/)
[![Practicum.Yandex](https://img.shields.io/badge/-Practicum.Yandex-464646?style=flat&logo=Practicum.Yandex&logoColor=56C0C0&color=008080)](https://practicum.yandex.ru/)
# PEP documentation parser for python

## Description
Python information parser for **https://docs.python.org/3/** and **https://peps.python.org/**

### Before use
Clone the repository to your computer using the commands:
```
git clone https://github.com/StanislavBerezovskii/bs4_parser_pep.git
```
or
```
git clone git@github.com:StanislavBerezovskii/bs4_parser_pep.git
```
or
```
gh repo clone StanislavBerezovskii/bs4_parser_pep
```

In the root folder create a virtual environment and install dependencies.
```
python -m venv venv
```
```
pip install -r requirements.txt
```
### change the directory to the ./src/ folder
```
cd src/
```
### run the main.py file selecting the required parser and arguments (shown below)
```
python main.py [parser option] [arguments]
```
### Built-in parsers
- whats-new   
Parser that displays a list of changes in python.
```
python main.py whats-new [arguments]
```
- latest_versions
A parser that displays a list of python versions and links to their documentation.
```
python main.py latest-versions [arguments]
```
- download   
Parser downloading zip archive with python documentation in pdf format.
```
python main.py download [arguments]
```
- pep
Parser that displays a list of pep document statuses
and the number of documents in each status. 
```
python main.py pep [arguments]
```
### Arguments
It is possible to specify arguments to change the operation of the program:  
- -h, --help
General information about teams.
```
python main.py -h
```
- -c, --clear-cache
Clearing the cache before parsing.
```
python main.py [parser option] -c
```
- -o {pretty,file}, --output {pretty,file}   
Additional data output methods
pretty - displays the command line data in a table
file - saves information in csv format in the ./results/ folder
```
python main.py [parser option] -o file
```
### Open Source License
GPL v3 (can check in gpl-3.0.md file)
### Author
- [Stanislav Berezovskii](https://github.com/StanislavBerezovskii "GitHub account")
