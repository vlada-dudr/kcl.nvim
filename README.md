# kcl.nvim

[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fkcl-lang%2Fkcl.nvim.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2Fkcl-lang%2Fkcl.nvim?ref=badge_shield)

Neovim KCL Extension

![image](https://github.com/kcl-lang/kcl.nvim/assets/462087/c5bcb1db-87a1-4ddb-ae7d-558f122a08e3)

## ⚡️ Requirements

### Manually:

Install the [kcl-language-server](https://kcl-lang.io/docs/user_docs/getting-started/install) from the binary.

> Don't forget to ensure it is in your `$PATH`, check the install location through the following command.

```shell
which kcl-language-server
```

### [mason.nvim](https://github.com/williamboman/mason.nvim):

Simply call `:MasonInstall kcl` to install the `kcl-language-server`

```
:MasonInstall kcl
```

## 📦 Installation

Install the plugin using your preferred plugin manager such as:

### [packer.nvim](https://github.com/wbthomason/packer.nvim):

```lua
use 'kcl-lang/kcl.nvim'
```

### [folke/lazy.nvim](https://github.com/folke/lazy.nvim):

```lua
require('lazy').setup({
  "kcl-lang/kcl.nvim",
})
```

### [vim-plug](https://github.com/junegunn/vim-plug)

```lua
local vim = vim
local Plug = vim.fn['plug#']

vim.call 'plug#begin'
Plug('kcl-lang/kcl.nvim')
vim.call 'plug#end'
```

## 🚀 LSP Config

Add this to `init.lua`:

```lua
require('lspconfig').kcl.setup({})
```

## ✨ Features

+ Syntax Highlight
+ Code folding
+ Quick Comment
+ Diagnostics: Warnings and errors in KCL file.

## 🍭 Commands

**Normal mode:**

```zC```  Close all folds under the cursor recursively. 

```zO```  Open all folds under the cursor recursively. 

```zM```  Close all folds.

```zR```   Open all folds. 

## License

[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fkcl-lang%2Fkcl.nvim.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2Fkcl-lang%2Fkcl.nvim?ref=badge_large)
