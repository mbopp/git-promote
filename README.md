git-promote
===========

Shell Script to help facilitate promoting from one environment (branch) to another

There are number of scripts out there that help developers deal with streamlining the version control process. This is one of them.  With a single command you can checkout a target branch and merge your development (or test) branch eventually committing and pushing the changes on the target branch.

usage
-----

The script makes some assumptions.  You may want to adapt it to your environment.  It assumes there are three environments, your **dev** (or develop), **review** (or test), and **production** (or master).

To move your code from your dev branch to review...   
`git promote review` or `git promote test`   

To move code from the review to production environment...   
`git promote production` or `git promote master`   

And that's it.  

caution
-------

This script presumes that you have committed your local dev changes before running the script.    

installation
------------

You simply need to move this script **git-promote** to somewhere in your executable path.  I personally have a **~./bin** directory that is on my path where I put custom scripts.

As you have noticed by the usage examples you do not need to put a dash in the name of the command even though that is the name of the script.  You can issue it just as you would any other git command.