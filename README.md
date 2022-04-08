# Terminal-Tools

An always growing set of terminal tools (command line applications).

List of the actual tools:
- WbSearch
- PreparePack
- TermClock

Before installing and using these tools and the relative commands, make sure that Python is in your PATH.

# WbSearch

Search anything on your main browser directly from terminal (both words and links).

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

Replace "keyword" with your own keyword, and "link" with your own link.
This method allows to locally set constant keywords. \
For example, typing:

    $ wbsearch -s youtube https://www.youtube.com/ 

Typing "wbsearch youtube", wbsearch will open the
saved link referring to "youtube" keyword.

`Remove method`:

    $ wbsearch --remove keyword

    $ wbsearch -r keyword

Replace "keyword" with the keyword you want to remove from wbsearch user keywords.

    $ wbsearch -r youtube

Typing "wbsearch youtube", youtube will be searched on your browser, but no longer the link associated to the keyword.

`Help`:

    $ wbsearch
    
Type "wbsearch" only with no arguments to get help.

# PreparePack

Repository that prepares packages directories and files

`Installation`:

    $ pip install preparepack

`Usage`:

    $ prepack packageName

Replace packageName with the name of your package. It will create the package directory named aspackageName_package, the setup.py file, a subdirectory named packageName containing the __ init __.py file and the package file named as packageName.py .

    $ buildpack 

Using this command you build the needed files before uploading your repository, such as .tar.gz and .whl . When you use this command, you must be in the same directory where the setup.py file is located.

    $ uploadpypi

Calling this command, you start the procedure for uploading a package on Pypi. Make sure to be in the the directory which contains the dist folder. Make also sure to have a valid Pypi account, to remember the credentials and that your package has a valid name (not taken yet) and a valid version (not uploaded yet).
# TermClock

`Installation`:

    $ pip install termclock
    
`Usage`:

    $ ctime
    
Shows a running clock in your terminal session. Press Ctrl+C to stop it.

    $ cdate
    
Shows current date, including the day of the week. Date format: DD/MM/YYYY

    $ cdatetime
    
Shows both current date and current time, with the running clock. Press Ctrl+C to stop it.
