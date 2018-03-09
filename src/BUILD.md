# How to build x64 Gvim with Visual Studio 2017

## Prerequisite

[Microsoft Windows SDK for Windows 7 and .NET Framework 4](https://www.microsoft.com/en-us/download/details.aspx?id=8279)
Remove *Microsoft Visual C++ 2010 Redistributable* if installation fails.

## Instruction
1. Open *x64 Native Tools Command Prompt for VS 2017*
2. Set *SDK_INCLUDE_DIR* environment variable
set SDK_INCLUDE_DIR=C:\Program Files\Microsoft SDKs\Windows\v7.1\Include
3. Run *nmake* with proper options
nmake -f Make_mvc.mak CPU=AMD64 CPUNR=i686 GUI=yes IME=yes MBYTE=yes DIRECTX=yes OLE=no NETBEANS=no XPM=no
