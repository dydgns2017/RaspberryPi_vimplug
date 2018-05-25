### 라즈베리파이에서 매니저 플러그인 vim-plug를 설치

## Install

업데이트 및 vim 다운로드 ( 라즈베리파이에 기본적으로 vim 편집기가 깔려있지 않음 ㅠㅠ )

```
sudo apt-get update && sudo apt-get install -y vim
sudo apt-get install -y vim-python-jedi
sudo apt-get install -y cmake
```

vim-plug 다운로드

```
curl -fLo ~/.vim/autoload/plug.vim --create-dirs \
    https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
```

## Configuration

기본적인 NERDTree, Syntastic, vim-airline 플러그인들이 설치됨.

```
cd ~/.vim
git clone https://github.com/dydgns2017/RaspberryPi_vimplug.git 
mv RaspberryPi_vimplug/.vimrc RaspberryPi_vimplug/.vimrc.local ~ 
vim "+:PlugInstall" 
```

```
## youcompleteMe Error Fix
cd ~/.vim/plugged/youcompleteme
./install.py
```

플러그인이 설치가 완료되면 :qa!로 vim을 종료시킨 뒤에 정상적으로 동작되는지 테스트해보세요 :D

## Reference
https://github.com/junegunn/vim-plug <br />
https://bluesh55.github.io/2016/10/09/vim-ide/ <br />
https://vimawesome.com/?q=cat%3Alanguage <br />
https://github.com/Valloric/YouCompleteMe/issues/914 <br />
