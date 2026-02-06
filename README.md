# dotfiles (WSL)

## Install
```bash
sudo apt-get update
sudo apt-get install -y stow git
./install/doctor.sh
./install/install.sh
```

## Manual install selected configs
### Neovim
1. Copy files:
* Linux/macOS: ```~/.config/nvim/init.lua```
* Windows: ```%LOCALAPPDATA%\nvim\init.lua```
2. Run *Neovim* and wait for plugins install complete
3. Inside *Neovim* execute command:
* ```:Mason``` → install ***rust-analyzer***, ***codelldb*** (for debugging)
* Ensure ```rustfmt`` and `clippy` are available (for example, from rustup):
    * ```rustup component add rustfmt clippy```
