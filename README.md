# YouCompleteMe Win64 已编译版本(ts-completer)
YouCompleteMe Windows 64已编译版本, 支持javascript补全, 更为详细的问题请移步[https://github.com/ycm-core/YouCompleteMe](https://github.com/ycm-core/YouCompleteMe)

## 编译环境
1. python 3.8.5 64位
2. Visual Studio 2017
3. cmake 3.18.2 64位
4. node 13.14 64位
5. npm 6.14.4
6. Windows 10

## 安装vim 64位，需要支持python3
https://github.com/vim/vim-win32-installer

## 编译时命令
```
git clone https://github.com/ycm-core/YouCompleteMe.git
cd YouCompleteMe
git submodule update --init --recursive
python install.py --clang-completer --ts-completer --msvc=15
```

## ycm安装或补充缺失的文件 
1. [必须]将 libclang.dll 复制一份到 ``YouCompleteMe/third_party/ycmd/third_party/clang/lib/``下面

## 编译时碰到问题
### 出现tsserver为空，无法继续编译
手动删除该目录，重新编译

