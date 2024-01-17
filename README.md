# VimTsunami
A WebStorm inspired config for Neovim





# Before we start
Vim is key-based text-editor.
All original keybinds from Vim are saved in this config. So, it's highly recommended to finish Neovim :Tutor first. 
Default \<leader\> key is \<space\>

# Installation

# Creating a project
You can create project from a boilerplate. 
List of available boilerplates: 
- Empty Project
- Angular CLI
- Bootstrap
- Express
- HTML5 Boilerplate
- Next.js
- Node.js
- React Native
- Vite
- Vue.js


# Write and edit source code

## Find action 
Find action using Telescope commands(see [Telescope commands](https://github.com/nvim-telescope/telescope.nvim?tab=readme-ov-file#vim-pickers))
Use <kbd>\<leader\>pa</kbd> to see list of available commands

![image](https://github.com/EngineerMonkey404/VimTsunami/assets/74253189/32fb49e1-2278-4763-b436-c72d79cc5126)

## https://www.jetbrains.com/help/webstorm/working-with-source-code.html#toggle-read-only

## Lines of code

- To add a line after the current one, press <kbd>o</kbd> in normal mode. It will move the caret to the next line.<br>
- To add a line before the current one, press <kbd>O</kbd> in normal mode. It will move the caret to the previous line.<br>
- To duplicate a line, press <kbd>Ctrl-d</kbd> in normal mode.<br>
- To delete a line, place the caret at the line you need and press<kbd>dd</kbd> in normal mode.<br>
- To join lines, place the caret at the line to which you want to join the other lines and press <kbd>J</kbd>.Keep pressing the keys until all the needed elements are joined.<br>
- To comment a line of code, place the caret at the appropriate line and press <kbd>gcc</kbd>. Press <kbd>gcc</kbd> again on the same line to uncomment it.
- To comment several lines of code, select few lines and press <kbd>gc</kbd>. Press <kbd>gc</kbd> on selected lines to uncomment them.
- To move a line up or down, select it, press <kbd>J</kbd> to move it down or <kbd>K</kbd> to move it up.
- To move (swap) an XML or HTML tag attribute to the left or to the right, place the caret at it, or select it and press CtrlAltShift0← for left or CtrlAltShift0→ for right. - ? 

## Copy and paste code

Understanding these terms will help you recall the correct keyboard shortcut.
- Y stands for “yank” in Vim, which is conceptually similar to copying.
- D stands for “delete” in Vim, which is conceptually similar to cutting.
- P stands for “put” in Vim, which is conceptually similar to pasting.

### Copying

- You can use <kbd>y</kbd> to copy selected text to Vim buffer.
- You can use <kbd>y</kbd> to copy selected text to Vim buffer.
- You can use <kbd>yy</kbd> to copy the whole line to Vim buffer.
- You can use <kbd>Y</kbd> to copy from caret to the end of line to Vim buffer.
- You can use <kbd>\<leader\>y</kbd> to copy selected text to system clipboard.
- You can use <kbd>\<leader\>Y</kbd> to copy from caret to the end of line to system clipboard.


### Cutting

- You can use <kbd>d</kbd> on selected text to cut it into Vim buffer.
- You can use <kbd>dd</kbd> to cut the line into Vim buffer.
- You can use <kbd>\<leader\>d</kbd> to cut the line into system clipboard.


### Pasting

- You can use <kbd>p</kbd> to put the data from Vim buffer after the cursor.
- You can use <kbd>P</kbd> to put the data from Vim buffer before the cursor.
- You can use <kbd>Ctrl-Shift-V</kbd> to put the data from system clipboard after the cursor.

By default, when you select text and paste something upon the selected text, selected text goes to Vim buffer.
To prevent it you can use <kbd>\<leader\>p</kbd>, so it will save what you have in Vim buffer.


### Troubleshooting:
If some commands above don't copy in to system clipboard, try to install [xsel](https://github.com/kfish/xsel) to your system. 


## Code selection
Use <kbd>v</kbd> to enter view mode and start selection.
Use <kbd>V</kbd> to enter view mode with line selection.


## Code statements 

### Move statements

Select needed code statement then use <kbd>H</kbd> or <kbd>J</kbd> to move it up or down.


#### Complete current statement

- Press <kbd>Ctrl-Space</kbd> in insert mode to start completion.
- Use <kbd>Ctrl-j</kbd> or <kbd>Ctrl-h</kbd> to select next or previous to choose relevant suggestion.
- Use <kbd>\<CR>\</kbd> after selection to complete statement.


## Code fragments

- Use <kbd>U</kbd> in visual mode to convert selected text to uppercase.
- Use <kbd>u</kbd> in visual mode to convert selected text to lowercase.
- Use <kbd>~</kbd> in visual mode to toggle case.
- Use <kbd>gc</kbd> to comment selected code fragment in visual mode.


## Code folding

- To toggle between fold and unfold, press <kbd>za</kbd>.
- To collapse or expand all code fragments, press <kbd>zM</kbd>/<kbd>zR</kbd> in normal mode.
- To collapse or expand code recursivly, press <kbd>zc</kbd>/<kbd>zo</kbd> in normal mode.
- To create custom folding region use <kbd>zf</kbd> on selected code in view mode to create foldable region in visual mode.
- To delete custom folding region use <kbd>zd</kbd> in normal mode.
- To delete custom folding region and all nested regions use <kbd>zD</kbd> in normal mode.
- To peek folded lines under cursor use <kbd>K</kbd> in normal mode.


# Editor basics

## Navigation

See [navigation between windows](https://neovim.io/doc/user/windows.html#window-move-cursor)


## Scrollbar

When you work this config displays code analysis results that include errors and warnings on the scrollbar. You can check whether your code has issues and quickly navigate to them.

For more information and customization check [nvim-scrollbar](https://github.com/petertriho/nvim-scrollbar)


## Editor tabs﻿

Every time you open a file for editing, a tab with its name is added next to the active editor tab.

### Close tabs

- To close only active tab use <kbd><A-c></kbd>
- To close all tabs except pinned use <kbd><leader>bwp</kbd>
- To close all tabs except current use <kbd><leader>bwc</kbd>
- To close all tabs except current and pinned tabs use <kbd><leader>bwe</kbd>
- To close all tabs on the left from current tab use <kbd><leader>bwl</kbd>
- To close all tabs on the right from current tab use <kbd><leader>bwl</kbd>


### Copy path or filename

- To copy relative path of current tab file use <kbd><leader>cf</kbd>
- To copy absolute path of current tab file use <kbd><leader>cF</kbd>
- To copy filename path of current tab file use <kbd><leader>ct</kbd>
- To copy directory name of current tab file use <kbd><leader>ch</kbd>


### Move or sort tabs

- To move tab to the left use <kbd></kbd>
- To move tab to the left use <kbd></kbd>
- To sort tabs by use <kbd></kbd>
- To sort tabs by use <kbd></kbd>
- To sort tabs by use <kbd></kbd>
- To sort tabs by use <kbd></kbd>






# List of plugins

| Plugin | Description |
| --- | --- |
| [Comment](https://github.com/numToStr/Comment.nvim) | Smart and Powerful commenting plugin for neovim |
| [nvim-ts-context-commentstring](https://github.com/JoosepAlviste/nvim-ts-context-commentstring) | A Neovim plugin for setting the commentstring option based on the cursor location in the file. |
| [vim-illuminate](https://github.com/RRethy/vim-illuminate) | Vim plugin for automatically highlighting other uses of the word under the cursor using either LSP, Tree-sitter, or regex matching. |
| [mason.nvim](https://github.com/williamboman/mason.nvim) | Portable package manager for Neovim that runs everywhere Neovim runs.Easily install and manage LSP servers, DAP servers, linters, and formatters. |
| [mason-lspconfig.nvim](https://github.com/williamboman/mason-lspconfig.nvim) | mason-lspconfig bridges mason.nvim with the lspconfig plugin - making it easier to use both plugins together. |
| [nvim-lspconfig](https://github.com/neovim/nvim-lspconfig) | Configs for the Nvim LSP client |
| [nvim-cmp](https://github.com/hrsh7th/nvim-cmp) | A completion engine plugin for neovim written in Lua. |
| [cmp-nvim-lsp](https://github.com/hrsh7th/cmp-nvim-lsp) | nvim-cmp source for neovim's built-in language server client. |
| [Luasnip](https://github.com/L3MON4D3/LuaSnip) | Dependency plugin for nvim-cmp |
| [project.nvim](https://github.com/ahmedkhalf/project.nvim) | project.nvim is an all in one neovim plugin written in lua that provides superior project management. |
| [nvim-web-devicons](https://github.com/nvim-tree/nvim-web-devicons) | Plugin to provide web-icons |






  

