`git-hop` provides easier access to a particular workflow inspired by a
file-backup system of working.

When using `git-hop`, your commit tree will look something like this:

           * ba
           |
    bb * * *
        \|/
         * * * a
         | |/
       b * *
          \|
           *
        master

That is, branches directly off of master are labelled a, b, c, etc., and
branches off of those have another letter appended to them.  Thus, you know
that the branch "aba" is the first branch off "ab", which is in turn the second
branch off "a", which is the first branch off master.

In this workflow, master is generally not the primary working branch.  Since it
is primarily designed for single-user single-computer work, the primary working
branch is whatever branch is currently active (checked out).

Usage
=====

`git hop [commit id]`

