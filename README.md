### 라즈베리파이에서 매니저 플러그인 vim-plug를 설치

## Install

업데이트 및 vim 다운로드 ( 라즈베리파이에 기본적으로 vim 편집기가 깔려있지 않음 ㅠㅠ )

```
sudo apt-get update && sudo apt-get install -y vim
```

vim-plug 다운로드

```
curl -fLo ~/.vim/autoload/plug.vim --create-dirs \
    https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
```

## Configuration

```

cp /etc/vim/vimrc ~/.vim/
cd ~/.vim
git clone ... ( 미정 )

vim+PlugInstall+q

```


## Reference
https://github.com/junegunn/vim-plug  \n
https://bluesh55.github.io/2016/10/09/vim-ide/
