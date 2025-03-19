# NeoVim Config
My nvim config that I use on my Windows machine.

## Plugins
Using,
    
- [lazy.nvim](https://github.com/folke/lazy.nvim.git): Plugin Manager
- [alpha-nvim](https://github.com/goolord/alpha-nvim.git): NeoVim Homepage
- [nvim-autopairs](https://github.com/windwp/nvim-autopairs.git): Makes using brackets easier
- [indent-blankline.nvim](https://github.com/lukas-reineke/indent-blankline.nvim.git): Indentation 
- [NvChad/nvim-colorizer.lua](https://github.com/NvChad/nvim-colorizer.lua): View colour codes. 
- [williamboman/mason.nvim](https://github.com/williamboman/mason.nvim): LSP Manager
- [williamboman/mason-lspconfig.nvim](https://github.com/williamboman/mason-lspconfig.nvim): Bridge for Mason and NeoVim LSP
- [neovim/nvim-lspconfig](https://github.com/neovim/nvim-lspconfig): NeoVim LSP
- [shortcuts/no-neck-pain.nvim](https://github.com/shortcuts/no-neck-pain.nvim): Auto-centre when using one buffer
- [hrsh7th/nvim-cmp](https://github.com/hrsh7th/nvim-cmp): Completion Engine
- [danymat/neogen](https://github.com/danymat/neogen): Auto-generate doxygen data. 
- [numToStr/Comment.nvim](https://github.com/numToStr/Comment.nvim): Commenting
- [ibhagwan/fzf-lua](https://github.com/ibhagwan/fzf-lua): Fuzzy file finding with grep, also installed some optional dependencies 
- [MeanderingProgrammer/render-markdown.nvim](https://github.com/MeanderingProgrammer/render-markdown.nvim): Live rendering of markdown files. 
- [folke/todo-comments.nvim](https://github.com/folke/todo-comments.nvim.git): Fancy TODO: comments 
- [nvim-treesitter/nvim-treesitter](https://github.com/nvim-treesitter/nvim-treesitter.git): Syntax Highlighting
- [mbbill/undotree](https://github.com/mbbill/undotree.git): Improved Undo
- [folke/which-key.nvim](https://github.com/folke/which-key.nvim.git): Key Hints
- [kevinhwang91/nvim-ufo](https://github.com/kevinhwang91/nvim-ufo.git): Folding
- [rmagatti/auto-session](https://github.com/rmagatti/auto-session.git): Session manager 

Colourscheme is my own in `colors/` and some fonts I like are in `fonts/`.

## Structure
Using `lazy.vim` to create a modular structure in `/lua`,

- `plugins/` contains all the plugin `.lua` files and the `/unused` directory for unused plugins.
- `manager.lua` to setup `lazy.vim`.
- `remaps.lua` for key remappings.
- `sets.lua` for general settings.

## Config Setup
### Windows
- Install NeoVim.
- Execute in terminal (Windows Powershell): `git clone https://github.com/ymich9963/nvim-config $HOME\AppData\Local\nvim` 

### Linux
- Install NeoVim using the AppImage to get the latest version.
- Execute in terminal: `git clone https://github.com/ymich9963/nvim-config ~/.config/nvim`. 

## Plugin Setup
- Run `:Lazy sync` to make sure everything is working

## Comments
- Setting up the LSP required combining the example given in the Mason docs by executing `:h mason-lspconfig-automatic-server-setup` and the [setup](https://github.com/hrsh7th/nvim-cmp?tab=readme-ov-file#setup) provided by `nvim-cmp`.

