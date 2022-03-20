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
# PL & tools list
### Java
- Java SE 17 [download](https://www.oracle.com/java/technologies/downloads/) and [install](https://docs.oracle.com/en/java/javase/17/install/installation-jdk-linux-platforms.html#GUID-4907E1A6-7B4B-4E98-9DA5-BF2A4D01AA57)
- Apache Maven [download](https://maven.apache.org/download.cgi) and [install](https://maven.apache.org/install.html)
- Installation summary
```shell
# extract java
tar zxvf jdk-17.INTERIM.UPDATE.PATCH_linux-x64_bin.tar.gz

# extract mvn
tar xzvf apache-maven-3.8.5-bin.tar.gz

# check env variable
echo $JAVA_HOME
/Library/Java/JavaVirtualMachines/jdk1.8.0_45.jdk/Contents/Home

# adding to PATH
export PATH=/opt/apache-maven-3.8.5/bin:$PATH
```
### Python
- python
```shell
sudo apt update
sudo apt install python3 python3-dev python3-venv
```
- pip
```shell
sudo apt-get install wget
wget https://bootstrap.pypa.io/get-pip.py
sudo python3 get-pip.py
```
### Golang
- Go latest [download](https://go.dev/doc/install)
```shell
# run as sudo
rm -rf /usr/local/go && tar -C /usr/local -xzf go1.18.linux-amd64.tar.gz
# add to PATH
export PATH=$PATH:/usr/local/go/bin
```
