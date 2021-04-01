# Default Settings Preview

![lua preview](./media/preview.png "Lua Preview")

# Introduction

`nvim-soluarized` is a colorscheme based on [`vim-solarized8`](https://github.com/lifepillar/vim-solarized8) and written with [`nvim-highlite`](https://github.com/Iron-E/nvim-highlite). It supports both light _and_ dark backgrounds. See __usage__ for more.

# Prerequisites

1. Neovim 0.5+

# Installation

1. Install a plugin manager such as [`packer.nvim`](https://github.com/wbthomason/packer.nvim) and use it to "plug" this repository.
	```viml
	use 'Iron-E/nvim-soluarized'
	```
2. Specify this colorscheme as your default colorscheme in the `init.vim`:
	```viml
	" Enable 24-bit color output. Only do this IF your environment supports it.
	" This plugin is fully compatible with 8-bit, 16-bit, and 24-bit colors.
	set termguicolors
	" Use the colorscheme
	colorscheme soluarized
	```

## Creating Your Own

1. Fork this repository, or clone it with `git clone https://github.com/Iron-E/nvim-soluarized`.
2. Follow the instructions in [`colors/soluarized.vim`](colors/soluarized.vim).
	* If you are on a Unix system, use the [setup script](setup.sh) like so:
	```sh
	chmod +x ./setup.sh
	./setup.sh soluarized <colorscheme>
	```
	Where `<colorscheme>` is the name of your desired colorscheme.
	* If you are on Windows, rename the files manually.

# Usage

To use a light or dark background with this colorscheme, simply `:set bg` in your `init.vim`, like so:

```vim
" for dark background
set bg=dark

" for light background
set bg=light
```

If you are using `init.lua`, use this statement instead:

```lua
-- for dark background
vim.o.background = 'dark'

-- for light background
vim.o.background = 'light'
```

See the [main repo](https://github.com/Iron-E/nvim-soluarized) for more usage tips.
