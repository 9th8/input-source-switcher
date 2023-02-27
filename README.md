Command line input source switcher for Mac.
===========================================

About
-----

This small utility for Apple OS X allows to easily switch input sources from a command line.
It's main purpose is to be used as a service in [vim-xkbswitch](https://github.com/lyokha/vim-xkbswitch) plugin.

Usage
-----

    issw [-h] [-l] [<input-source-id>]

    -h - show help message
    -l - list all selectable input sources
    -V - print version number

    If no arguments are specified, it prints the current input source.
    If <input-source-id> is specified, it selects the specified input source.

How to build
------------

    git clone git@github.com:9th8/input-source-switcher.git
    cd input-source-switcher
    mkdir build && cd build
    cmake ..
    make
    mkdir -p ~/.local/lib
    mv libInputSourceSwitcher.dylib ~/.local/lib/
