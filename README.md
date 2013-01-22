bash_tools
==========

A collection of usefull bash tools, easing daily tasks on the command line.

DESCRIPTION
-----------

For detailed information which functions etc. are provided through these
files, take a look at the describing comments of each file.

INSTALL
-------

Copy over all `.bash_tools*`-files in your home directory and add following
lines to your `.bashrc`:

    if [ -f ~/.bash_tools ]; then
        . ~/.bash_tools
    fi

If you want to see the status of the tools (enabled/disabled) add following
to your `.bashrc`:

    if [ -f ~/.bash_tools ]; then
        # check if logged in with (1) ssh or (2) sftp
        if [ "$0" != '-bash' ] && [ "$0" != 'bash' ]; then
            BASH_TOOLS_VERBOSE=1
        fi
        . ~/.bash_tools
        unset BASH_TOOLS_VERBOSE
    fi

For detailed information concerning configuration see .bash_tools

