# QieQt

Customized version of Qt 6 source code used in QieLive project.

This work based on [Mile.Qt](https://github.com/ProjectMile/Mile.Qt) but the
source code tree is rebased.

Huge thanks to [Yuhang Zhao](https://github.com/wangwenx190) for his patch.
This patch makes us only need to release Qt 6 version of QieLive project only,
and still support Windows 7 Service Pack 1.

## Differences from Mile.Qt

We select LGPLv3 only for our customized version. This is why we don't include
any Qt components which cannot distributed under LGPLv3.

We only provide the x64 target compilation script because QieLive project only
supports the x64 target.

## Usage

First, you need the Visual Studio 2022 or later, with C++ workload installed.

Then, you need to download the latest [VC-LTL release]. Extract the VC-LTL
binary package to the place what you want and execute the `Install.cmd` for it.

[VC-LTL release]: https://github.com/Chuyu-Team/VC-LTL5/releases

And you need to execute `apply-patches.bat` to apply the necessary patch.

After that, you can execute `onekey-build-x64.bat` to compile our customized
version, execute this script in the console or terminal window you created is
recommend because you can see the detailed result information in the end.
