# Terminal-Tools

An always growing set of terminal tools (command line applications).

List of the actual tools:
- WbSearch
- PreparePack
- TermClock

Before installing and using these tools and the relative commands, make sure that Python is in your PATH.

# WbSearch

Installation
    
    $ pip install wbsearch
    
Usage:

    $ wbsearch argument
    
  Replace argument with the words or the link you want to search. If you are searching multiple words, put "\" before each space, or wrap the around with double quotes.

    $ wbsearch --set keyword argument
    
    $ wbsearch -s keyword argument
    
  The --set method, allows to create keywords for WbSearch. Replace keyword with your own keyword, and argument with the link you want to save. After this operation, by typing "wbsearch keyword", you will search the link associated with the keyword.

# PreparePack

Installation:

    $ pip install preparepack
    
This library creates templates for repository/libraries building.

Usage:

    $ prepack -n projectName
    
Replace projectName with your own project name. 
This command will create (inside the current folder), a directory called "projectName_package", inside of the which will be created: a setup.py file (with some template code), a directory named as your project name containing the __init__.py file and a blank python file called as your project name.

    $ buildpack
    
This command must be called only inside the directory containing setup.py. When called, it installs locally the module, and creates .tar.gz and .whl files.
After calling it, you can try and use (locally) your repository.

# TermClock

Installation:

    $ pip install termclock
    
Usage:

    $ ctime
    
Shows a running clock in your terminal session. Press Ctrl+C to stop it.

    $ cdate
    
Shows current date, including the day of the week. Date format: DD/MM/YYYY

    $ cdatetime
    
Shows both current date and current time, with the running clock. Press Ctrl+C to stop it.
