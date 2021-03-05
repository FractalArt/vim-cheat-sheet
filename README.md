# Vim Cheatsheet

This repository contains my personal vim cheatsheet, listing the commands that I use most frequently. The document is subdivided according to the modes in vim.

******

## Normal mode

### Searching

| Command | Comment |
| :-----: | :-----: |
| / | launch the search process |
| n | move the cursor to the next match. |
| N | move the cursor to the previous match. |
| * | find the next occurence of the word under the cursor |
| # | find the previous occurence of the word under the cursor |

### Undo and Redo

| Command | Comment |
| :-----: | :-----: |
| u | undo the last edit |
| Ctrl + r | redo the last edit |


### Entering insert mode
| Command | Comment |
| :------: | :-----: |
| i | insert content before the current character |
| a | insert content after the current character |
| A | insert content at the end of the line |
| o | open a new line, below the current one and switch to insert mode |
| O | open a new line, above the current one and switch to insert mode |

### Moving around

Move horizontally:

| Command | Comment |
| :-----: | :-----: |
| w | move cursor to the next word |
| b | move cursor to the previous word |
| e | move cursor to the end of the current word |
| 0 | move cursor to the beginning of the line |
| ^ | move to the first non-blank character of the current line |
| $ | move to the end of the current line |
| % | move to the matching bracket when the cursor is already on a bracket |
| f<character> | find a character after the cursor |
| F<character> | find a character before the cursor |
| t<character> | move till a character after the cursor |
| T<character> | move till a character before the cursor |
| ; or , | to move to the next and previous character chosen in the previous two commands, respectively |

Moving vertically:

| Command | Comment |
| :-----: | :-----: |
| <line number> G | move your cursor to the beginning of an arbitrary line |
| G | move the cursor to the last line of the file |
| gg | move the cursor to the first line of the file |
| 1G | move the cursor to the first line of the file |
| Ctrl + e | scroll downwards |
| Ctrl + u | move the cursor upward half a screen |
| Ctrl + d | move the cursor downward half a screen |

One can enter a word several times from normal mode by tying `<number>i<word> Esc`.

### Windows, Buffers and Tabs

Splitting the window horizontally can be done by typing `:sp {filename}` andvertically by typing `:vsp {filename}`. Moving between panels can be done
by typing `Ctrl + W + h/j/k/l`.

Opening a new tab is achieved by typing `:tabnew {fileame}`.
Moving to the next tab is done through typing `gt`, the previous tab is reached through `gT` and a numbered tab is obtained through `{n}gt`.

A new buffer can be opened by typing `:new {filename}`. Moving between buffers is equivalent to moving between windows.
A list of all buffers can be displayed by typing `:ls`. One can access the buffer with number `n` through `:b {n}`.

### Editing text

| Command | Comment |
| :-----: | :-----: |
| x | delete the character under the cursor |
| r<character> | replace the character under the cursor with the provided character |
| dw | delete until the end of the current word under cursor | 
| d<n>w | delete until the end of the <n>th word starting from the word under the cursor |
| diw | delete inside the current word, i.e. delete current word |
| dd | remove the current line |
| p | paste content removed with `d` |
| y | yank / copy the selected text |
| . | repeat the previous command |

******

## Visual mode

| Command | Comment |
| :-----: | :-----: |
| Shift+v | select the line under the cursor. |

A lot of the standard `vim` commands that we have seen above can be applied to the selection.

******

## References

- [Is Vim Really Not For You? A Beginner Guide](https://thevaluable.dev/vim-beginner/)
- [A Vim Guide For Intermediate Users](https://thevaluable.dev/vim-intermediate/)
- [A Vim Guide For Advaced Users](https://thevaluable.dev/vim-advanced/)
- [Interactive Vim Tutorial by OpenVim](https://www.openvim.com/tutorial.html)
- [TypeRacer](https://play.typeracer.com/)
- [Sokoban](https://matthieucneude.com/sokoban/)
- [Snake](https://matthieucneude.com/snake/)
