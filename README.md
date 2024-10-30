# Setup

Dear future me, I did not track all of the dependencies, but some are:

- `fish`
- `zellij`
- `nvim 0.10.0`
- `fzf`, `ripgrep`, `fd`
- `npm`
- `clang`, use it to build a nvim telescope extension
- `go` install `delve` for dap config
- `rust`
- `python` - needs `venv` to be installed

In `Mason`, `markdownlint` needs to be installed.

## Change bashrc to fish

I used `chsh`

## Sync `dotfiles/` with configs

TODO: I should fix this script to be smarter

```bash
ln -s ~/dotfiles/nvim ~/.config/nvim
ln -s ~/dotfiles/.tmux.conf ~/.tmux.conf
ln -s ~/dotfiles/starship.toml ~/.config/starship.toml
ln -s ~/dotfiles/.mybashrc ~/.mybashrc
```

## Include custom gitconfig

In `~/.gitconfig`:

```md
[include]
    path = dotfiles/.mygitconfig
```
