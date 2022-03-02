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

> Now only support one git address ,  Multi-address will support later.

2. Easier color output

```shell
#before
echo -e "\033[33m\n\tConfiguration Information : \n\033[0m"
#now
color red "Erro" "bad message."
```

3. Updating …

## Install and Uninstall

1. clone

```shell
git clone https://github.com/guodong52cc/shellFuncLib.git
```

2. install

```
cd shellFuncLib
chmod +x install
. install
```

3. uninstall

```shell
chmod +x unintall
. unintall
```

