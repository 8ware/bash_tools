bash_tools
==========

A collection of usefull bash tools, easing daily tasks on the command line.

DESCRIPTION
-----------

### .bash_tools

This file provides some useful methods to develop bash tools. It further
`source`s all "subfiles" (beginning with `.bash_tools_`).

### .bash_tools_git

This utility file extends common command line tools, like `git`, `mv` or
`rm` with a context sensitiv behavior. For example the `mv`-command invokes
the `git mv`-command if the current directory is a Git-repository. For more
information about the provided functionality have a look at the comments
in that file.

INSTALL
-------

Copy over all `.bash_tools*`-files in your home directory and add following
lines to your `.bashrc`:

  if [ -f ~/.bash_tools ]; then
      . ~/.bash_tools
  fi

For detailed information concerning configuration see .bash_tools

