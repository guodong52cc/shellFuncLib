# shellFuncLib
shell ( bashrc / zshrc ) function library

## Function

1. One command to achieve using proxy to git push your git

```shell
#before
export http_proxy=xxxxxxx
export https_proxy=xxxxxxx
git add .
git commit -m [message]
git push
#now
gdpush [message]
```

Use:
```shell
# add your git into config.yaml
vim config.yaml
# update git command
gitfunc update
# remove git and reinit gitcommand
gitfunc reupdate
# eg:(name of "type: git" in config is gd)
gdpush [message] #git push
gdpush  #git push (read inputs)
gdpush HELP #help
gdpush CHECK #git and proxy infomation
gdpush PROXY #system proxy status
gdpush CLEAN #reset system proxy
# or (name of "type: git" in config is sfl)
sflpush [message]
#......
```

2. Easier color output

```shell
#before
echo -e "\033[33m\n\tConfiguration Information : \n\033[0m"
#now
color red "Erro" "bad message."
```

3. parse_yaml

support shell parse yaml file

```shell
parse_yaml [file] [prefix]
#eg:
$ cat 1.yaml
apple: shop
    color: red
    size: 30px
gun: 
    color: brown

$ parse_yaml 1.yaml conf_
conf_apple="shop"
conf_apple_color="red"
conf_apple_size="30px"
conf_gun_color="brown"
```

4. Updating

## Install and Uninstall

1. clone

```shell
git clone https://github.com/guodong52cc/shellFuncLib.git
```

2. install

```
cd shellFuncLib
chmod +x install
. ./install
```

3. uninstall

```shell
chmod +x unintall
. ./uninstall
```

