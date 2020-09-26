## setup nodenv

1. install anyenv
```
brew install anyenv
```
2. add script to .zshrc
```
echo 'eval "$(anyenv init -)"' >> .zshrc
```
3. exec anyenv init
```
anyenv install --init
```
4. reload shell
```
zsh -l
```
5. install nodenv
```
anyenv install nodenv
```
6. mkdir nodenv plugin directory
```
mkdir -p "$(nodenv root)/plugins"
```
7. add nodenv-yarn-install plugin
```
git clone https://github.com/pine/nodenv-yarn-install.git "$(nodenv root)/plugins/nodenv-yarn-install"
```
8. install node
```
nodenv install 14.12.0
```
9. set global node version
```
nodenv global 14.12.0
```
10. confirm
```
node -v
v14.12.0
```
```
yarn -v
1.22.5
```
