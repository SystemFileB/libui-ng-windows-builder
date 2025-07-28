# libui-ng-windows-builder
在Actions中编译libui-ng

你可以从Actions->构建->最新的一次提交->Artifacts中下载编译好的libui-ng

libui/bin目录下所有exe文件在实际开发的时候可以不用带上

## 版本说明
build-\<MSYSTEM\>-[deps]

MSYSTEM: 
- MINGW64: 64位的libui-ng
- MINGW32: 32位的libui-ng
- UCRT64: 64位的libui-ng，Windows 8.1及以前的系统必须使用deps版本
- CLANGARM64: ARM64的libui-ng，但是它现在还无法编译，所以没有这个版本

deps: 如果有这个标志就表明它带上了依赖库，但是这里并没有包含UCRT

Linux只有build-x86_64，build-aarch64两个版本