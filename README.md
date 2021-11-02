# VScode-environment
***Visual Studio Code***
- 关于编译运行C/C++的调试配置
---
## 编译器安装
要先安装好你要用的编译器，比如TDM-GCC，MinGW，Clang，MSVC

最关键的一步就是设置好*PATH*

打开控制面板->系统与安全->系统->(左边)高级系统设置->环境变量->选择Path编辑->添加你安装编译器源目录的bin文件夹

当按下win+R，运行cmd，输出``gcc -v``或``g++ -v``回车之后出现一堆东西就是设置Path成功了

---
## C/C++调试配置
打开VScode，选择菜单栏 文件->打开文件夹，选择一个你认为合适的文件夹

然后是 查看->命令面板->输入关键词"C/C++ edit"->选择"C/C++: Edit Configurations (UI)", 确定编译器路径正确、IntelliSence模式正确

之后随便创建一个C/CPP，随便写个代码

然后选择菜单栏 运行->添加配置->按需选择(MSVC选Windows，其他应该选GDB/LLDB)

然后选择默认的 "***.exe-生成和调试活动文件"

这样就完事了，可以使用VScode的调试功能了

---
## json文件的备注
"program" 是编译后生成的exe保存的路径

"miDebuggerPath" 是编译器的路径

变量名查看
[CSDN社区](https://blog.csdn.net/bailsong/article/details/77527773)  或者  [啃生肉？](https://stackoverflow.com/questions/38703278/vscode-environment-variables-besides-workspaceroot)
