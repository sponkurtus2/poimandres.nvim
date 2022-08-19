<div align="center">
  <img src="https://user-images.githubusercontent.com/47901349/182481495-06f11e94-8d8a-4580-b869-56b6defae182.png" width="100px">      
  <h1>poimandres.nvim</h1>
</div>

<p align="center">
  <a href="#">
    <img alt="Made with Lua" src="https://img.shields.io/badge/Made%20with%20Lua-00359F.svg?style=for-the-badge&logo=lua" style="vertical-align:center" />
  </a>
</p>

Neovim theme with the palette of [poimandres vscode theme](https://github.com/drcmda/poimandres-theme), written in Lua with treesitter support. 

All variants of the theme will be available for use.

![Poimandres Golang](https://user-images.githubusercontent.com/47901349/185516934-6db42b76-bd96-4b3f-8c20-058827b6c70f.png)

<details>
<summary>More screenshots</summary>

### Lua

![Poimandres Lua](https://user-images.githubusercontent.com/47901349/182434460-3702a751-7cc1-43c6-aa9e-05843ad5489c.png)

### TypeScript

![Poimandres TypeScript](https://user-images.githubusercontent.com/47901349/182434594-0e8b3408-92ec-4056-8907-9a28a94fa08a.png)

### Golang

![Poimandres Golang](https://user-images.githubusercontent.com/47901349/182434263-91489ea7-8e6f-4c2a-b738-6d3f293cd357.png)

</details>

### Plugin Support

- [TreeSitter](https://github.com/nvim-treesitter/nvim-treesitter)
- [LSP Diagnostics](https://neovim.io/doc/user/lsp.html)
- [LSP Trouble](https://github.com/folke/lsp-trouble.nvim)
- [Git Signs](https://github.com/lewis6991/gitsigns.nvim)
- [Telescope](https://github.com/nvim-telescope/telescope.nvim)
- [NvimTree](https://github.com/kyazdani42/nvim-tree.lua)
- [Indent Blankline](https://github.com/lukas-reineke/indent-blankline.nvim)
- [Lualine](https://github.com/hoob3rt/lualine.nvim)

_More plugins will be supported as I personally need it, or when it is requested._

## 📦 Installation

Install with [packer](https://github.com/wbthomason/packer.nvim):

```lua
-- Lua

use { 
  'olivercederborg/poimandres.nvim',
  config = function()
    require('poimandres').setup {
      -- leave this setup function empty for default config
      -- or refer to the configuration section
      -- for configuration options
    }
  end
}
```

Install with [vim-plug](https://github.com/junegunn/vim-plug):
```vim
" Vim Script

Plug 'olivercederborg/poimandres.nvim'

lua << EOF
  require('poimandres').setup {
    " leave this setup function empty for default config
    " or refer to the configuration section
    " for configuration options
  }
EOF
```

## 🚀 Usage

**Enable the colorscheme**:

```lua
-- Lua

vim.cmd('colorscheme poimandres')
```

```vim
" Vim Script

colorscheme poimandres
```

## ⚙️ Configuration:

**Setup function options**: 

```lua
{
  bold_vert_split = false, -- use bold vertical separators
  dim_nc_background = false, -- dim 'non-current' window backgrounds
  disable_background = false, -- disable background
  disable_float_background = false, -- disable background for floats
  disable_italics = false, -- disable italics
}
```

To enable Poimandres for `Lualine`, just set the theme in your Lualine configuration:

```lua
require('lualine').setup {
  options = {
    -- ... your lualine config
    theme = 'poimandres'
    -- ... your lualine config
  }
}
```

## 🙌 Related

- [poimandres-theme](https://github.com/drcmda/poimandres-theme): VSCode version
- [poimandres-alacritty](https://github.com/z0al/poimandres-alacritty): Alacritty version
- [poimandres-iterm](https://github.com/alii/poimandres-iterm): Iterm version
- [poimandres-wezterm](https://github.com/olivercederborg/poimandres-wezterm): Wezterm version

### Hyper theme

```bash
hyper i hyper-pmndrs
```
