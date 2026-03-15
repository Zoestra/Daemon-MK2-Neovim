# Daemon MK2

A deep red and cyan color scheme for Neovim, inspired by the Cyberpunk 2077 terminal theme and the [Daemon mk2 KDE Theme](https://github.com/MathisP75/daemon-kde-mk2).

This theme is built using [Lush](https://github.com/rktjmp/lush.nvim), a Neovim plugin for creating color schemes.

## Features

- Dark theme with deep red and cyan accents
- Designed for readability and a cyberpunk aesthetic
- Supports Neovim's built-in syntax highlighting
- Compatible with Tree-Sitter and LSP

![Screenshot of example code in Neovim using the Daemon-MK2-Neovim theme](/Daemon-mk2-neovim-screenshot.png)

## Requirements

- Neovim 0.5 or later
- [lush.nvim](https://github.com/rktjmp/lush.nvim)

## Installation

### Using [Packer](https://github.com/wbthomason/packer.nvim)

Add this to your `init.lua`:

```lua
use {
  'Zoestra/Daemon-MK2-Neovim',
  requires = {'rktjmp/lush.nvim'}
}
```

Then run `:PackerInstall`.

### Using [Vim-Plug](https://github.com/junegunn/vim-plug)

Add this to your `.vimrc` or `init.vim`:

```vim
Plug 'rktjmp/lush.nvim'
Plug 'Zoestra/Daemon-MK2-Neovim'
```

Then run `:PlugInstall`.

### Using [lazy.nvim](https://github.com/folke/lazy.nvim)

Add this to your `init.lua`:

```lua
{
  "Zoestra/Daemon-MK2-Neovim",
  dependencies = { "rktjmp/lush.nvim" },
}
```

Then run `:Lazy sync`.

### Manual Installation

Clone the repository into your Neovim configuration directory:

```bash
git clone https://github.com/Zoestra/Daemon-MK2-Neovim.git ~/.config/nvim/pack/plugins/start/daemon-mk2-neovim
```

Make sure [lush.nvim](https://github.com/rktjmp/lush.nvim) is also installed.

## Usage

After installation, set the colorscheme in your `init.lua`:

```lua
vim.cmd('colorscheme daemon')
```

Or in your `.vimrc`:

```vim
colorscheme daemon
```

## Customization

The theme is defined in `lua/lush_theme/daemon.lua`. You can modify the colors and highlighting groups there. After changes, reload Neovim or run `:Lushify` if you have lush installed.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Credits

- Inspired by [Daemon mk2 KDE Theme](https://github.com/MathisP75/daemon-kde-mk2)
- Built with [Lush](https://github.com/rktjmp/lush.nvim)

## AI Disclosure

The initial creation of this theme was done by a human, the conversion into a useable plugin, and the creation of this README was performed by AI.
If any errors are found, please open an issue, and I will take care of it.
