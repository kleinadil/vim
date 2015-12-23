# How to build x64 Gvim with Visual Studio 2015

## Prerequisite

[Microsoft Windows SDK for Windows 7 and .NET Framework 4](https://www.microsoft.com/en-us/download/details.aspx?id=8279)
Remove *Microsoft Visual C++ 2010 Redistributable* if installation fails.

## Instruction
1. Open *VS2015 x64 Native Tools Command Prompt*
2. Set *SDK_INCLUDE_DIR* environment variable
set SDK_INCLUDE_DIR=C:\Program Files (x86)\Microsoft SDKs\Windows\v7.1\Include
3. Run *nmake* with proper options
nmake -f Make_mvc.mak CPU=AMD64 CPUNR=i686 GUI=yes IME=yes MBYTE=yes DIRECTX=yes OLE=no NETBEANS=no XPM=no
