# vim-scavenger

Multiple empty lines and trailing white spaces cleaner for Vim.

Vim-scavenger supports both Vim and [Neovim](https://neovim.io/).

## Requirement

### Vim

Need Python 2.x support for Vim. Check with the following command: `vim --version | grep "+python"`.

### Neovim

Install [neovim/python-client](https://github.com/neovim/python-client). Currently, Just install the client of Python 2.x.

## Functions

### CleanUp()

`:call CleanUp()`

Delete all multiple empty lines and trailing spaces.

### CleanUpMultipleEmptyLines()

`:call CleanUpMultipleEmptyLines()`

Delete all multiple empty lines.


### CleanUpTrailingSpaces()

`:call CleanUpTrailingSpaces()`

Delete all trailing spaces.


### ScavengerHighlightAll()

`:call ScavengerHighlightAll()`

Highlight all empty lines and trailing spaces with red color.


### ScavengerClearHighlight()

`:call ScavengerClearHighlight()`

Clear all highlight on all empty lines and trailing spaces.


### ScavengerToggleHighlight()

`:call ScavengerToggleHighlight()`

Toggle highlight.

## Settings

### `g:scavenger_enable_highlight`

Enable to highlight when open files or not .

- default value: `1`
- value `1`: Highlight all multiple empty lines and trailing spaces when open files.
- value `0`: Do not highlight multiple empty lines and trailing spaces when open files.

### `g:scavenger_auto_clean_up_on_write`

Enable to clear multiple empty lines and trailling spaces when save files or not.

- default value: `0`
- value `1`: Clear multiple empty lines and trailing spaces when save files automatically.
- value `0`: Do not clear multiple empty lines and trailing spaces when save files automatically.