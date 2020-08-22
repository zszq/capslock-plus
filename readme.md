
## 前言 ##
​		**capslock-plus-rise** 是根据CapsLock+[（作者版本）](https://github.com/wo52616111/capslock-plus)和CapsLockPlus（CapsLock+修改版）[（CapsLockPlus版本）](https://github.com/PatrickShieh/CapsLockPlus)再次修改，在两位作者的布局和功能基础上尽量保持原布局和功能的同时进行了优化，以适合自己日常使用。如果是经常用键盘输入文字（如程序员），相信你在半天时间就能完全上手。

​		感谢CapsLock+开源这款工具， 2020-04-25作者重新更新了，但是新的布局很不友好，交流了一下，作者说有时间了会继续优化，可以关注并打赏原作者[（开源作者）](https://github.com/wo52616111/capslock-plus)。

​		如CapsLockPlus作者所说：本人是个键盘党，还是个程序猿，非常不喜欢敲代码敲得嗨时，还要去碰鼠标、右手移动一段距离去操作方向键，删除键等等。噢，对了，还很讨厌Ctrl键，因为使用Ctrl组合键时，左手要离开键盘一段距离，神烦。试想下，双手不用离开字母区，是不是很爽，嘿嘿。



>capslock+rise：[下载地址](https://github.com/zszq/capslock-plus-rise/releases/tag/1.0.0)



**已知可能会出现的问题：**
1、**启动之后不报错按键没有任何反应，请查看360等安全软件是否拦截了模拟按键，并加入白名单！！！**
2、ctrl + v 进行粘贴时会出现 ctrl不起作用，只有v键起作用了。 解决方法：删除 v键输出的内容重新粘贴，或者用软件带的 capslock + v 进行粘贴。
3、其他问题请查看 [原文档](https://capslox.com/capslock-plus/#使用)



**以下内容引用CapsLockPlus作者的介绍页面，只作简要说明。**更多详情请查看 [原文档](https://capslox.com/capslock-plus/)

## 概述 ##

CapslockPlus是一个加强 Capslock 键的功能，以提高效率的工具。让你拥有更多的组合键，例如：

- CapsLock + 全键
- CapsLock + Alt + 全键
- CapsLock + Shift + 全键



## 版本对比 ##

>CapsLock按键省略为Caps，Key为各种按键，下面对比的是大功能模块，小功能到原作者文档查看。

功能| CapsLock+（原版） | CapsLockPlus（修改版） | CapsLock+rise（自用版） 
:-:                 | :-:   | :-: |:-:                 
Caps + Key          | <font color="#00dd00">✔</font>     | <font color="#00dd00">✔</font>     | <font color="#00dd00">✔</font> 
Caps + Alt + Key    | <font color="#00dd00">✔</font>     | <font color="#00dd00">✔</font>     | <font color="#00dd00">✔</font> 
Caps + Shift + Key  | <font color="#dd0000">✘</font>     | <font color="#00dd00">✔</font>| <font color="#00dd00">✔</font> 
Caps + Ctrl + Key   | <font color="#dd0000">✘</font>     | <font color="#00dd00">✔</font>| <font color="#dd0000">✘</font>（按键不便不添加） 
TabScript           | TabScript     | TabSnippet| TabScript 
WinBind             | <font color="#00dd00">✔</font>     | <font color="#00dd00">✔</font>| <font color="#00dd00">✔</font> 
QBar                | <font color="#00dd00">✔</font>     | <font color="#dd0000">✘</font> | <font color="#00dd00">✔</font>（原作者4月最新版） 
TransplatePanel     | <font color="#00dd00">✔</font>     | <font color="#00dd00">✔</font>| <font color="#00dd00">✔</font> （增加谷歌翻译国内版） 
DAAS                | <font color="#dd0000">✘</font>     | <font color="#00dd00">✔</font>| <font color="#dd0000">✘</font>（个人用处不大不添加） 



## 按键说明 ##

如布局图片挂了可查看complete文件夹内图片，或者用浏览器查看文件hotkey_layout.html。

#### 1. Caps + Key ####
>以下省略了CapsLock键，默认是要加上的，未设置功能键的可自行设置。

![3Fc2I.png](https://wx1.sbimg.cn/2020/08/23/3Fc2I.png)

**1.1 CapsLock + 鼠标**

按键| 功能说明
:-:| :-:
鼠标左键|✘
鼠标中键|✘
鼠标右键|✘
鼠标滚轮向前|音量加
鼠标滚轮向后|音量减

#### 2. Caps + Alt + Key
>以下省略了CapsLock + Alt键，默认是要加上的，未设置功能键的可自行设置。

[![3FdLK.png](https://wx2.sbimg.cn/2020/08/23/3FdLK.png)](https://sbimg.cn/image/3FdLK)

**2.1 CapsLock + Alt + 鼠标**（临时改变鼠标速度，并在松开后复原，默认是3，范围是1~20。）

按键| 功能说明
:-:| :-:
鼠标左键|✘
鼠标中键|✘
鼠标右键|✘
鼠标滚轮向前|加快按下 Capslock+LAlt 时鼠标的速度
鼠标滚轮向后|降低按下 Capslock+LAlt 时鼠标的速度

#### 3. Caps + Shift + Key
>以下省略了CapsLock + Shift键，默认是要加上的，未设置功能键的可自行设置。

![3FsMT.png](https://wx1.sbimg.cn/2020/08/23/3FsMT.png)

**3.1 CapsLock + Shift + 鼠标**

按键| 功能说明
:-:| :-:
鼠标左键|双显示器有效，将当前软件移动到另外显示器
鼠标中键|✘
鼠标右键|✘
鼠标滚轮向前|✘
鼠标滚轮向后|✘



> 以下功能只作简要说明，除 **WinBind** 有变动外，其他详细说明参考 [原文档](https://capslox.com/capslock-plus/#advancedFunctions)

## TabScript 热字符串

#### 按键
    CapsLock + Tab

>### 功能
>
>1. 光标左边的字符串如果在`Capslock+settings.ini`文件[1]中的`[TabHotString]`，`[QRun]`或`[QWeb]`字段下有相应键名，则将其替换成该键名对应的值
>2. 计算光标左边的数学表达式的值（实际上是运行`JavaScript`代码，参考原作者文档）
>
>### 说明
>
>- 关于热字串功能：
> 1. 举个例子，在`Capslock+settings.ini`文件的`[TabHotString]`段下有这么一条设置：`email=123456789@abc.com`，那么在任意能输入文字的地方输入：`asdfghjkl**email**`，按下`Capslock+Tab`，就会变成`asdfghjkl**123456789@abc.com**`
>
> 2. 如果不同字段下有同名的键名，三个标签的优先级是：
>    `[TabHotString]` > `[QRun]` > `[QWeb]`
>    例如：
>    `[TabHotString]`段下有设置：`a=apple`
>    `[QRun]`段下有设置：`a=e:\banana`
>    那么输入`a`后，`Capslock+Tab`将得到`apple`（而不是`e:\banana`）
>    （虽然理论上不同段名下的键名可以同名，但`[QRun]`和`[QWeb]`下的键名不应重名，否则在使用`+Q`功能时会有问题）
> - 关于计算功能：参考 [原文档](https://capslox.com/capslock-plus/#clTabScript)



## WinBind ##

#### 如何绑定
    绑定窗口:CapsLock + Alt + (`或1~8)

<ul>
  <li>模式1：单击，绑定当前激活的窗口到相应按键；</li>
  <li>模式2：双击，追加绑定当前激活的窗口到相应按键；</li>
  <li>模式3：三击，绑定当前激活的窗口所属程序所拥有的所有窗口到相应按键;</li>
</ul>

#### 如何激活
    激活窗口:CapsLock + (`或1~8)
>### 功能
>
>1. `激活`/`最小化`绑定在该按键的窗口
>
>### 说明
>
>- 关于绑定：
>  1. 模式1和模式3会覆盖当前按键上已有的绑定窗口
>  2. 模式2绑定在按键现有模式是模式1或模式2时会追加窗口，是模式3时不追加，而会覆盖原绑定设置，绑定当前激活窗口（与模式1效果一样）
>  3. 模式2操作示例：
>     1. 激活窗口A（鼠标点击一下是方法之一），依次按下`Capslock``Alt`不放，再按两次`1`；
>     2. 激活窗口B，同样操作；
>     3. 激活窗口C，同样操作；
>     4. 按下`Capslock`不放，（多次）按下`1`来在A,B,C三个窗口之间实现类似`Alt+Tab`的窗口切换。
>  4. 模式2绑定的窗口被关闭至只剩下1个时，将自动转换成模式1绑定（可以激活 / 最小化窗口）
>- 关于窗口激活 / 最小化：
>  1. 模式1下，在原窗口不存在时，激活动作会自动绑定窗口所属程序的另一个窗口
>  2. 模式1和模式3下，在原绑定窗口所属程序未启动时，激活动作将启动该程序
>  3. 绑定的窗口只有一个时，所有模式都将激活 / 最小化该窗口



## Qbar

    绑定窗口:CapsLock + Q

>### 功能
>
>1. 弹出输入框，输入不同命令执行不同操作（见下面的`cl` `set`等）
>
>### 说明
>
>1. 按下`ESC`键或失去焦点后将关闭界面
>2. 选中字符再按下`+Q`可以将其填入输入框
>3. 选中文件再按下`+Q`，它的路径会填入输入框



## 如何自行设置全局的按键

>在CapsLock+settings.ini里[Keys]设置，请对照CapsLock+settingsDemo.ini 来配置相关设置，里面说的很详细
