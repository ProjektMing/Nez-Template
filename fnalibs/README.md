# fnalibs

## 说明

`fnalibs` 是 FNA 的一个依赖库集合，包含了 FNA 运行所需的所有库文件。
该文件夹下存放的库文件可以通过 MSBuild 自动选择当前平台所需的文件，并放在编译产物目录下，不过目前仅写了 Windows 下的逻辑(仅有 x86 和 x64)。

编译前，请在 [GitHub](https://github.com/FNA-XNA/fnalibs-dailies/actions) 获取最新的 CI 内容并解压置于在[当前目录下](./)。
