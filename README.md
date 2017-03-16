# matlab.vim

# Description 
matlab.vim is a vim script which aims to easy to edit matlab.vim scripts,the 
**Features** cotains as following:

    1. keywords highlight (common words,not all)
    2. Automatic alignment
    3. Check syntax error
    4. Tag support
    5. jump matching groups

However, I am a just a porter, this script is made by someone in matlab forum.

**It only for linuxer!**

## How to install it ?
if you you are using **vundle** , you could add following to vundle configure in
~/.vimrc:
```
Plugin "yinflying/matlab.vim"
```
and then update the vundle in vim :
```
:PluginInstall
```
of course, you could also download these file and then put then under ~/.vim/

And then you should add following in ~/.vimrc to support syntax checking:
```
autocmd BufEnter *.m    compiler mlint
```
of cousrse, you should have the "mlint" , which provide by matlab. You could
check by type "mlint" in terminal. If not recognized, you should fint the file 
"mlint" under the matlab directory , and make a link under /usr/bin;

if you want use "%" to match if/end,classdef/end,methods/end,you should install 
another plugin "matchit".
## How to use it ?
You could automatic alignment with "=";

You could check the systax error by ":make" and ":copen", and ":cn"&":cp" jump 
to error line;
