# Bible of vim
Cool things about vim.

# Must have plugins
+ [vim-plug](https://github.com/junegunn/vim-plug) - *Old*
+ [packer.nvim](https://github.com/wbthomason/packer.nvim) - **Recommended**
+ [coc.nvim](https://github.com/neoclide/coc.nvim)
+ [fzf.vim](https://github.com/junegunn/fzf.vim) - *Old*
+ [telescope.nvim](https://github.com/nvim-telescope/telescope.nvim) - **Recommended**
+ [vim-surround](https://github.com/tpope/vim-surround)
+ [vim-fugitive](https://github.com/tpope/vim-fugitive)
+ [ultisnips](https://github.com/SirVer/ultisnips) 
+ [auto-pairs](https://github.com/jiangmiao/auto-pairs)

# Color schemes
+ [lucidity](https://github.com/usirin/lucidity)
+ [bleed-purple](https://github.com/usirin/bleed-purple.nvim) - **Recommended**
+ [Gruvbox](https://github.com/morhetz/gruvbox)
+ [Gruvbox Community](https://github.com/gruvbox-community/gruvbox)
+ [vim-gruvbox8](https://github.com/lifepillar/vim-gruvbox8) - **Recommended**
+ [Spaceduck](https://github.com/pineapplegiant/spaceduck)
+ [Moonfly](https://github.com/bluz71/vim-moonfly-colors)
+ [Lucid](https://github.com/cseelus/vim-colors-lucid)
+ [Jellybeans](https://github.com/nanotech/jellybeans.vim)
+ [night-owl](https://github.com/haishanh/night-owl.vim)
+ [tokyonight](https://github.com/folke/tokyonight.nvim)
+ [tender](https://github.com/jacoborus/tender.vim)
+ [srcery](https://github.com/srcery-colors/srcery-vim)
+ [badwolf](https://github.com/sjl/badwolf)
+ [xcode](https://github.com/arzg/vim-colors-xcode)

# Recipes
+ tmux + nvim true color issue solution
  ```
  " init.vim
  let &t_8f = "\<Esc>[38;2;%lu;%lu;%lum"
  let &t_8b = "\<Esc>[48;2;%lu;%lu;%lum"
  let $NVIM_TUI_ENABLE_TRUE_COLOR=1
  ```
  ```
  # .tmux.conf
  set -g default-terminal 'screen-256color'
  set -ga terminal-overrides ',*256col*:Tc'
  ```
+ Key macro
  + Type `qa` in `normal` mode to record. (`a` is our register that we save our key presses)
  + Do your thing.
  + Back to normal mode. Press `q` to stop recording. 
  + Type `@a` or you can type `x@a` to do `x` times the same thing.
+ Open vim directly in fugitive `nvim -c 'G | wincmd j | hide' .`
+ `:stop` suspend and `fg` revoke
+ `ctrl + g` see the full filename
+ `q:` see command history
+ `<C-w>T` move to tab
+ `Shift-Up to Ctrl-Y and Shift-Down to Ctrl-E`
+ `:set statusline=%{synIDattr(synIDtrans(synID(line('.'),col('.'),1)),'name')}` see the hlgroup under the cursor.
+ `ma` mark the position to a register then `'a` to get back to the marked position.
+ to start vim in sudo mode with your config, add this line to your .zshrc or .bashrc
   ```
      export SUDO_EDITOR="nvim"
   ``` 
+ `J` concat the lines
+ `:verbose map <C-i>` debug the keymap
+ `ctrl-o` | `ctrl-i` jump between "jump list", a list of places where your cursor has been to
+ `gf` go file
+ useful `netrw` keybindings
  + `p` preview file
  + `t` open in new tab
  + `r` reorder
  + `d` make directory
  + `i` change view mode
  + `shift+cr` expand folder in tree view
+ `:read` yank from a file and paste directly to the current file
+ A `buffer` is a value and a `window` contains the reference of a buffer.
+ When you need to rememder a autocmd look here http://vimdoc.sourceforge.net/htmldoc/autocmd.html

# Cool talks
+ Mastering the Vim Language https://www.youtube.com/watch?v=wlR5gYd6um0
+ How to Do 90% of What Plugins Do (With Just Vim) https://www.youtube.com/watch?v=XA2WjJbmmoM
