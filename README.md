gilog2timesheet
===============

gitlog2timesheet is a tool to general timesheet from git logs. 

Usage
-----

        Usage: gitlog2timesheet.py path_to_git_repo(s) ...

        Options:
          -h, --help            show this help message and exit
          -d, --debug           output debug messages
          -w COMMITFACTOR, --commitfactor=COMMITFACTOR
                                work time factor per commit, default is 4 hours

Sample output
-------------


        gitlog2timesheet.py /home/adulau/git/forban

        From Mon Apr  9 15:12:02 2012 to Mon Apr  9 16:12:02 2012
           Alexandre Dulaunoy (a@foo.be) worked on forban
            and did the following: Fixed #12 test if loot directory exists

        From Mon Apr  9 13:30:30 2012 to Mon Apr  9 14:30:30 2012
           Alexandre Dulaunoy (a@foo.be) worked on forban
            and did the following: Fixed #9 lootcleanup added

        From Mon Apr  9 12:41:42 2012 to Mon Apr  9 13:41:42 2012
           Alexandre Dulaunoy (a@foo.be) worked on forban
            and did the following: Fixed #10 The browsing is now naturally sorted.

        From Sun Apr  8 10:35:10 2012 to Sun Apr  8 11:35:10 2012
           Alexandre Dulaunoy (a@foo.be) worked on forban
            and did the following: Fixed #7 cleanup mode added

Software required
-----------------

* Python 2.4 and up
* git

Note
----

Usually assuming that a commit has an amount of time spent on it is usually wrong.

But the tool is usually used for organizational structure requiring timesheet in a
strict format like who did what and when. You have been warned.
