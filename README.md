nano

GNU nano is a text editor for Unix-like operating systems

Details at https://www.nano-editor.org/

This port requires the enhanced realpath in zoslib for the filebrowser to work properly.
The patch for the ncurses library might be needed because of a mistake in the ncurses port, since it puts ncurses.h in ncurses/ncurses.h

Use the ncurses port to generate a terminfo database, export TERMINFO='location of terminfo' and export TERM=xterm-256color for example

Setting up syntax highlighting is possible by adding the syntax files in ~/.nanorc
For example to highlight shell scripts, c code and python add:

```
include nano-7.0/syntax/sh.nanorc
include nano-7.0/syntax/c.nanorc
include nano-7.0/syntax/python.nanorc
```

The syntax files are in the sourcecode distribution at https://nano-editor.org/dist/v7/
