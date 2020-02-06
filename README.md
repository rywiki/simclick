# SimClick 模拟点击

*一直以来，我总是以键盘控自居，应该是在从前做模型的时候伤到了手指关节开始，成为键盘重度用户的。各种键盘加速工具，主动去记住各种快捷键，力求少用鼠标，甚至去学习了vim和emacs。但是，很多时候，鼠标是无可替代的，尤其是在图形界面大行其道时候。*

## 概述



本工具将整个屏幕网格化，通过键盘进行鼠标的定位，并模拟鼠标的左键单击，右键单击和双击功能，能够实现在双手不离开键盘的情况下，快速跳转鼠标并实现点击。



## 操作方式



**1、启动**

双击程序图标运行。运行后，程序会在系统托盘位置显示图标，右键点击图标，可以看到以下内容的菜单：

* 配置（Config）：点击后，显示配置对话框；

* 关于（About）：点击后，显示功能介绍信息；

* 退出（Exit）：点击后退出程序。



**2、定位**

按下快捷键(当前为Shift+Space)呼叫出软件界面：

按照界面上的区域敲击键盘上对应的字母，对应的字母和单元格高亮（自左上角一次沿着横纵坐标顺序以A～Z命名单元格），鼠标移动到单元格中心位置	；

如果位置正确，可以模拟鼠标点击；

如果位置有偏离，敲击空格（Space），进入到微调界面；

以同样的方式敲击屏幕上对应位置的字母（横纵均分为4份，分别以左手默认手指位键（A、S、D、F）顺序命名），红线十字会定位到相应的位置，可以开始模拟鼠标点击。

在定位过程中任意时候按下Esc，取消定位过程。

Tip 1：定位字母的键入是循环输入的，依次输入两个字母键，如果定位的不是你所需的网格，仅需要重新输入即可，但注意当前输入的位置（每次都是两个字母输入来定位一个单元格，但每一次输入都会反映到界面中，如果出现某次单数输入，会造成输入顺序颠倒的感觉，暂无太好的解决方法）。

Tip 2：整体定位和微调定位之间可以通过空格进行切换，如果发现网格选择有错，微调定位无法定位到需要位置，可以按下空格键，重新进行整体定位。

Tip 3：由于采用的是windows窗体实现，因此网格窗体有可能在呼出之后被切入后台，但仍然显示在最前端，外观上没有区别，请不要在呼出网格窗体后进行其他窗体切换操作，如发生此类问题，请使用Alt+Tab将网格窗体切换到前台并关闭（按下Esc）。（此问题后期想办法解决）

**3、 点击**

当前版本可以模拟以下鼠标点击方式：

左键单击：回车（Return）；

右键单击：Ctrl+Return；

左键双击：Alt+Return.



## 已知问题

1. 在某些非windows窗体的应用程序（Delphi,QT）上，模拟点击无效或异常，定位功能尚可用；

2. 在某些封装桌面程序（Electron程序）中无法呼出网格窗体；

3. 在1920X1080分辨率下，底部和右侧有部分内容无法涵盖到主定位网格中（在微调定位阶段可以采用右手默认手指位键（J、K、L、;）进行扩展定位）；

4. 不支持跨虚拟桌面调用；

5. 暂未支持多屏幕。

   

##　支持

存在任何问题，请在issues中提出。纯业余时间作品，无法保证及时回复解答，请各位谅解。




