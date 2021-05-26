# Bible of vim
Cool things about vim.

# Must to have plugins
+ [vim-plug](https://github.com/junegunn/vim-plug)
+ [coc.nvim](https://github.com/neoclide/coc.nvim)
+ [fzf.vim](https://github.com/junegunn/fzf.vim)
+ [vim-surround](https://github.com/tpope/vim-surround)
+ [vim-fugitive](https://github.com/tpope/vim-fugitive)

# Color schemes
+ [Gruvbox](https://github.com/morhetz/gruvbox)
+ [Gruvbox Community](https://github.com/gruvbox-community/gruvbox)
+ [Spaceduck](https://github.com/pineapplegiant/spaceduck)
+ [Moonfly](https://github.com/bluz71/vim-moonfly-colors)
+ [Lucid](https://github.com/cseelus/vim-colors-lucid)
+ [Jellybeans](https://github.com/nanotech/jellybeans.vim)
+ [night-owl](https://github.com/haishanh/night-owl.vim)
+ [tokyonight](https://github.com/folke/tokyonight.nvim)
+ [tender](https://github.com/jacoborus/tender.vim)
+ [srcery](https://github.com/srcery-colors/srcery-vim)+ 
+ [badwolf](https://github.com/sjl/badwolf)

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

# Cool talks
+ Mastering the Vim Language https://www.youtube.com/watch?v=wlR5gYd6um0
