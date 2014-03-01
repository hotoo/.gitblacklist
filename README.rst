GIT - Pre-Commit check for certain words
----------------------------------------

:Author: Nikolaos Dimopoulos <nikos@niden.net>
:Thanks to: Remigijus Jarmalavicius <remigijus(at)jarmalavicius.lt>

About
-----
GIT pre-commit hook for checking the existence of certain words/phrases/functions 
in the code to be committed. These phrases are taken from external files, based on
the extension of the file being checked.

Example\: to check for "TODO" or "FIXME" in a java file, create the file ``{git root}/.precommitblacklist.java`` containing the two lines:

    | TODO
    | FIXME

How to install
--------------
To install hook, copy pre-commit file to your project .git/hooks/pre-commit:

    | $ cp pre-commit .git/hooks/pre-commit;
    | $ chmod +x .git/hooks/pre-commit;

The hook comes with no ``.precommitblacklist.EXTENSION`` files.

Bugs
----
For any bugs, please visit:

    https://github.com/niden/Git-Pre-Commit-Hook-for-certain-words/issues
