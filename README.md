# Terminal-Tools

An always growing set of terminal tools of my creation (command line applications).

List of the actual tools:
- [WbSearch](https://github.com/CargoCodes/Terminal-Tools/blob/main/README.md#wbsearch)
- [PreparePack](https://github.com/CargoCodes/Terminal-Tools/blob/main/README.md#preparepack)
- [TermClock](https://github.com/CargoCodes/Terminal-Tools/blob/main/README.md#termclock)
- [Winux](https://github.com/CargoCodes/Terminal-Tools/blob/main/README.md#winux)

Before installing and using these tools and the relative commands, make sure that Python is in your PATH.

# WbSearch

[Repository Link](https://www.github.com/CargoCodes/WbSearch)

Search anything on your main browser directly from terminal (both words and links).

    Version: 2.1.3

`Installation`:

    $ pip install wbsearch

`Usage`:

    $ wbsearch argument

Replace argument with your own research.
In case you want to search multiple words, you may need to use "\" before each space,
or use double quotes around, depending on your operating system. 

`Set method`:

    $ wbsearch --set keyword link

    $ wbsearch -s keyword link

Replace keyword with your own keyword, and link with your own link. 
This method allows to locally set constant keywords.
The same method allows to edit the content of the keyword, simply entering the keword and then the new associated link 

For example, typing:

    $ wbsearch -s youtube https://www.youtube.com/ 

Typing "wbsearch youtube", wbsearch will open the
saved link referring to "youtube" keyword.

`Remove method`:

    $ wbsearch --remove keyword

    $ wbsearch -r keyword

Replace "keyword" with the keyword you want to remove from wbsearch user keywords.

Example:

    $ wbsearch -r youtube

Typing "wbsearch youtube", youtube will be searched on your browser, but no longer the link associated to the keyword.

`Help`:

    $ wbsearch --help

Type this command to get help.

# PreparePack

[Repository Link](https://www.github.com/CargoCodes/PreparePack)

Repository that prepares packages directories and files

    Version: 1.4.0

`Installation`:

    $ pip install preparepack

`Usage`:

    $ prepack packageName

Replace packageName with the name of your package. It will create the package directory named aspackageName_package, the setup.py file, a subdirectory named packageName containing the __ init __.py file and the package file named as packageName.py .

    $ buildpack 

Using this command you build the needed files before uploading your repository, such as .tar.gz and .whl . When you use this command, you must be in the same directory where the setup.py file is located.

    $ uploadpypi

Calling this command, you start the procedure for uploading a package on Pypi. Make sure to be in the the directory which contains the dist folder. Make also sure to have a valid Pypi account, to remember the credentials and that your package has a valid name (not taken yet) and a valid version (not uploaded yet).

All commands have "--help" option.

# TermClock

[Repository Link](https://pypi.org/project/termclock/)

    Version: 1.1.0

`Installation`:

    $ pip install termclock
    
`Usage`:

    $ ctime
    
Shows a running clock in your terminal session. Press Ctrl+C to stop it.

    $ cdate
    
Shows current date, including the day of the week. Date format: DD/MM/YYYY

    $ cdatetime
    
Shows both current date and current time, with the running clock. Press Ctrl+C to stop it.

# Winux

[Repository Link](https://www.github.com/CargoCodes/winux)

Integration of some Linux terminal commands for Windows Command Prompt.

This CLA is in costant update with new command.

`Warning! Installing this library in a Linux OS or in a OS X (mac) machine may cause system commands overriding, 
which could become a serious problem. The code is ment to not work in non-Windows systems, but in Unix OSes it could 
overwite and"hide" the commands it provides.`

    Version: 1.1.3  

`Installation`:

    $ pip install winux

This Command Line Application allows to use Linux terminal commands in Windows Command Prompt.


`Integrated commands`: 
    
      Linux        Windows              Function

    $ clear         (cls)               Clear terminal window

    $ ls            (dir)               Show directory content

    $ mv            (move)              Move a file into another directory, or rename it

    $ cp            (copy)              Copy a file into another directory

    $ rm            (del)               Remove a file
    
    $ rm -rf        (rmdir)             Remove a directory

    $ cat           (type)              Show file content

    $ pwd           (chdir)             Shows current path

    $ date          (time)              Shows date and time

    $ nano          (edit)              Edit a file

    $ mem           (free)              Display free space

    $ kill          (taskkill)          Kill a process

    $ man           (?/)                Shows help for commands

    $ mkdir         (md)                Make a directory

    $ ps x          (tasklist)          Show running tasks

