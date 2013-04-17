=====================
    Launch Agents
=====================

These are some launchd_ jobs that I wrote to automate the running of
various little Unix-y tools I like to start when I log in to my box.

.. _launchd: https://en.wikipedia.org/wiki/Launchd

Usage
-----

Copy the job you want to use into your ``~/Library/LaunchAgents``
directory. It should run the next time you log in. If you would like to
start it up now, you should load the job using ``launchctl``, e.g.,

::

    $ launchctl load ~/Library/LaunchAgents/bcvi.plist

The Jobs
--------

``bcvi.plist``
    This simple job starts the bcvi_ listener process and keeps it alive.
    Obviously, if you haven't installed ``bcvi``, this isn't much use to you.

.. _bcvi: http://search.cpan.org/~grantm/App-BCVI-3.08/lib/App/BCVI.pm

Caveats
-------

I've only tested these jobs using my personal Mac (running Mountain Lion
and the version of perl_ you can get from Homebrew_).

.. _perl: http://www.perl.org
.. _Homebrew: http://mxcl.github.io/homebrew/
