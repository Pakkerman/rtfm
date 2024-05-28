# RTFM - Nvim

- [x] usr_01.txt - About the manuals
- [x] usr_02.txt - The first steps in Vim
- [x] usr_03.txt - Moving around
  - w and W has a difference, w is every stop at the edge of 2 kinds of word while chad W goes through the next blank and then stop
  - marks are cool and very confusing
- [x] usr_04.txt - Making small changes
- [x] usr_05.txt - Set your settings
- [x] usr_06.txt - Using syntax highlighting
- [x] usr_07.txt - Editing more than one file
- [x] usr_08.txt - Splitting windows
- [x] usr_09.txt - Using the GUI
- [x] usr_10.txt - Making big changes
- [x] usr_11.txt - Recovering from a crash
- [x] usr_12.txt - Clever tricks

## Editing Effectively

- [x] usr_20.txt - Typing command-line commands quickly
- [x] usr_21.txt - Go away and come back
- [x] usr_22.txt - Finding the file to edit
- [x] usr_23.txt - Editing other files
- [x] usr_24.txt - Inserting quickly

#### Fancy insert mode commands

- i_CTRL-X_CTRL-K: you can use to do completion with dictionary, you have to enable spelling to do this.
- i_CTRL-X_CTRL-O: OmniFunc with it's same as intellsense in other ides
- i_CTRL-R: open reg and insert stuff
- i_CTRL-O: Allows you to do a normal command then be put back to insert mode

- [x] usr_25.txt - Editing formatted text

#### Navigate horizontally

- zh: scroll right
- zH: scroll half a window width right
- ze: scroll right to put the cursor at the end
- zl: scroll left
- zL: scroll half a window width left
- zs: scroll left to put the cursor at the start

- [x] usr_26.txt - Repeating

- $ls | vim - : read from stdin and open in vim

- [x] usr_27.txt - Search commands and patterns

  - "a.\{-\}b" will match "axb" in "axbab"
  - "/forever\&..." will match "for", this pattern is forever, and dots are chars to match from the start, so 3 dots three chars. Hence "for" is matched, other word like "format" will not be match because there is no "forever" to be found
  - when using range patterns like "\s", "\a", adding "\_", "\_s" and "\_a" will also match a line break "\n". matches the pattern or a line break.
  - "\d" and "[0-9]" is the same, but \d is faster. Use that if speed is a concern.

- [x] usr_28.txt - Folding

  - zm: fold more (m for more)
  - zr: fold less (r for reduce)

- [x] usr_29.txt - Moving through programs

  - it seems like that the tags are largely being replaced by the LSP capabilities.

- [x] usr_30.txt - Editing programs

  - i_CTRL-T: indent current line with 'shiftwidth'

- [x] usr_31.txt - Exploiting the GUI

  - nvim doesn't really have GUI version, or it is the GUI hybrid version already?

- [ ] usr_32.txt - The undo tree

## Tuning Vim

- [ ] usr_40.txt - Make new commands
- [ ] usr_41.txt - Write a Vim script
- [ ] usr_42.txt - Add new menus
- [ ] usr_43.txt - Using filetypes
- [ ] usr_44.txt - Your own syntax highlighted
- [ ] usr_45.txt - Select your language (locale)

#### To watch outputs

- redir >> file to output stuff, then use tail -f to watch it

#### Useful keymaps

- gm: to move to the middle
- zs: to left align the column
- c_CTRL-R_CTRL-W: paste what is under the cursor

#### Useful commands

- command | vim - : read from stdin and open in vim
