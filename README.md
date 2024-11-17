# README

## This is a customized nvim config taken from https://github.com/LunarVim/Neovim-from-scratch.git ~/.config/nvim 

## If you want to start a fresh please try out

```
git clone https://github.com/LunarVim/Neovim-from-scratch.git ~/.config/nvim
```

## This config uses Neovim v0.10.2

**NOTE** [Mason](https://github.com/williamboman/mason.nvim) is used to install and manage LSP servers, DAP servers, linters, and formatters via the `:Mason` command.

## Get healthy

Open `nvim` and enter the following:

```
:checkhealth
```

You'll probably notice you don't have support for copy/paste also that python and node haven't been setup

So let's fix that

First we'll fix copy/paste

- On mac `pbcopy` should be builtin

- On Ubuntu

  ```
  sudo apt install xsel
  ```

- On Arch Linux

  ```
  sudo pacman -S xsel
  ```
  
- Wayland users

  [wl-clipboard](https://github.com/bugaevc/wl-clipboard)


Next we need to install python support (node is optional)

- Neovim python support

  ```
  pip install pynvim
  ```

- Neovim node support

  ```
  npm i -g neovim
  ```
---

**NOTE** make sure you have [node](https://nodejs.org/en/) installed, I recommend a node manager like [nvm](https://github.com/nvm-sh/nvm).

## To-Do

1. Replace packer with [lazy.nvim](https://github.com/folke/lazy.nvim)
2. Re-write the plugins configs and re-structure the whole code.
