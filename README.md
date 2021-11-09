![alah-copy](https://user-images.githubusercontent.com/6236123/140812913-ccad531c-2f55-4ef8-908e-bba2387da714.jpg)

first of all see some screen shot:

<img width="1671" alt="Screen Shot 1400-08-18 at 00 19 33" src="https://user-images.githubusercontent.com/6236123/140816097-850f4503-6fe2-4db8-8b12-9a201a6974c2.png">

# Pre Request

### Recomadation :

- we heighly recommand useing `Linux` or `Mac` as your operation system.

- [using `Wezterm` as your default Terminal emulator.](https://github.com/wez/wezterm)

  It is GPU-accelerated cross-platform terminal emulator and multiplexer written by @wez and implemented in Rust

  [It's my `wezterm.lua`](https://raw.githubusercontent.com/hemedani/dotfiles/main/wezterm/wezterm.lua), you should put it in `$HOME/.config/wezterm/wezterm.lua` :

- [using `Fish SHELL` as your default Shell.](https://github.com/fish-shell/fish-shell)

  It is he user-friendly command line shell.

- [using `starship` as you default Shell prompt.](https://github.com/starship/starship)

  It is the minimal, blazing-fast, and infinitely customizable prompt for any shell!

  [It's my `starship.toml`](https://raw.githubusercontent.com/hemedani/dotfiles/main/starship.toml), you should pu it in `$HOME/.config/starship.toml`

# Installing :

- install `Rust` with the help of [own doc](https://www.rust-lang.org/tools/install)

- install `Node JS`, [using fnm](https://github.com/Schniz/fnm) for install nodejs please (it's so fast)

- install `Deno` with the help of [own doc](https://deno.land/#installation)

- install `Neovim` and `Lua` [neovim and lua](https://github.com/neovim/neovim/wiki/Installing-Neovim), please install nightly version of neovim and install LuaJit

### Installing Formatter :

The major problem of IDE or IDE-Like performance relate to formating document. So we try to speed up this procces as much as possible.

We trying to format document with utils writen in rust `RUST`

- [install `dprint`](https://github.com/dprint/dprint) and set it to your `$PATH` :

  Pluggable and configurable code formatting platform written in Rust.

  [It's my `dprint.json`](https://raw.githubusercontent.com/hemedani/dotfiles/main/dpript/dprint.json) file, you should put it in `$HOME/.config/dotfiles/dpript/dprint.json`

- [install `stylua`](https://github.com/JohnnyMorganz/StyLua) and set it to your `$PATH` :

  An opinionated Lua code formatter written in rust

- install `prettier` globally: `npm i -g prettier` (sorry for using this shamefull lib we need it just for a few filetype)

### Install LSPs :

`Deno` and `Rust` LSP are installed and attaching to related buffer when you execute `nvim` command on proper root project;

- for installing `tsserver` LSP just run : `npm install -g typescript typescript-language-server` read the rest of it's doc [here](https://github.com/neovim/nvim-lspconfig/blob/master/CONFIG.md#tsserver)

- for installing `sumneko_lua` LSP read [this doc](https://github.com/sumneko/lua-language-server/wiki/Build-and-Run) and [this doc](https://github.com/neovim/nvim-lspconfig/blob/master/CONFIG.md#sumneko_lua)

### Setting Up:

- copy or clone this repo to `.config/nvim` :

  `git clone https://github.com/MiaadTeam/lesvim.git ~/.config/nvim`

- install plugins :
  - `:PackerInstall`
  - `:PackerCompile`

after lunching neovim install these `TreeSitter` lib with `TSInstall` :

- `TSInstall tsx`