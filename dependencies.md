# Installing Neovim
```bash
curl -LO https://github.com/neovim/neovim/releases/latest/download/nvim.appimage
sudo chmod +x nvim.appimage
sudo mkdir -p /usr/local/nvim 
sudo mv nvim.appimage /usr/local/nvim/nvim.appimage
sudo ln -s /usr/local/nvim/nvim.appimage /usr/local/bin/nvim 
```

# LSP Dependencies
```bash
go install golang.org/x/tools/gopls@latest
sudo npm i -g vscode-langservers-extracted
sudo npm i -g pyright
curl -fLo .config/nvim/autoload/plug.vim --create-dirs https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
```
