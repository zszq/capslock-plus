## 前言

　　感谢CapsLock+开源这款工具，和作者交流了一下，说有时间会继续优化，可以关注并打赏原作者[（开源作者）](https://github.com/wo52616111/capslock-plus)。

　　2020-04-25作者重新更新，但新的布局很不友好，于是用了三四天时间看了下autohotkey，并在最新版本的基础上对其进行了一些更改，以适合自己日常使用。

　　修改初衷，如CapsLockPlus作者所说：本人是个键盘党，还是个程序猿，非常不喜欢敲代码敲得嗨时，还要去碰鼠标、右手移动一段距离去操作方向键，删除键等等。噢，对了，还很讨厌Ctrl键，因为使用Ctrl组合键时，左手要离开键盘一段距离，神烦。试想下，双手不用离开字母区，是不是很爽，嘿嘿。

　　例如：选中文字 → `CapsLock+Q` → `CapsLock+space` 便自动打开浏览器显示百度搜索结果；按住`CapsLock`滚动鼠标滚轮就可调节音量等。

<br>


　　**CapsLockHotkey** 是参考CapsLock+（原版）和CapsLockPlus的布局（CapsLock+另一个修改版），尽量保持原布局和功能的同时进行了再次修改和优化。如果是经常用键盘输入文字（如程序员），相信你在半天时间就能完全上手。

<br>

CapsLockHotkey：[下载地址](https://github.com/zszq/CapsLockHotkey/releases)

<br>

### 已知可能会出现的问题：

1. **启动之后不报错按键没有任何反应，请查看360等安全软件是否拦截了模拟按键，并加入白名单！！！**
2. `ctrl + v` 进行粘贴时会出现 ctrl不起作用，只有v键起作用了。 解决方法：删除 v键输出的内容重新粘贴，或者用软件自带的 `capslock + v` 进行粘贴，或者`capslock + f8`关闭软件自带复制粘贴功能。
3. 通过`Ctrl+Alt+Capslock`快捷键启动 CapsLockHotkey，在桌面使用快捷键不起作用。解决方法：请激活任意软件后使用快捷键启动，或者双击软件启动。如果已经在桌面按了快捷键，在激活软件情况下还是没反应，请先切换下capslock键再重新尝试。如果在桌面使用快捷键造成切换大小写相反，请再次在桌面使用`Ctrl+Alt+Capslock`快捷键操作一次。（此bug待作者修复，推荐将其固定到开始菜单，通过点击启动。）
4. IDEA的默认快捷键有点奇葩，比如`ctrl+y`这些，所以此软件部分操作在IDEA上可能出现问题（测试小括号，中括号，大括号，尖括号会出问题，影响不大，用shift默认操作方式可解决），其他大部分操作没有任何问题，如有需要也可自行参考文档修改。
5. 其他问题请查看 [原文档](https://capslox.com/capslock-plus/#使用)

<br>

以下部分内容引用CapsLockPlus作者的介绍页面，只作简要说明。更多详情请查看 [原文档](https://capslox.com/capslock-plus/)

## 概述 ##

CapsLockHotkey是一个加强 Capslock 键的功能，以提高效率的工具。让你拥有更多的组合键，例如：

- CapsLock + 全键
- CapsLock + Alt + 全键
- CapsLock + Shift + 全键



## 版本对比 ##

>CapsLock按键省略为Caps，Key为各种按键，下面对比的是大功能模块，小功能到原作者[文档](https://capslox.com/capslock-plus/)查看。

功能| CapsLock+ | CapsLockPlus | CapsLockHotkey 
:-:                 | :-:   | :-: |:-:                 
Caps + Key          | <font color="#00dd00">✔</font>     | <font color="#00dd00">✔</font>     | <font color="#00dd00">✔</font> 
Caps + Alt + Key    | <font color="#00dd00">✔</font>     | <font color="#00dd00">✔</font>     | <font color="#00dd00">✔</font> 
Caps + Shift + Key  | <font color="#dd0000">✘</font>     | <font color="#00dd00">✔</font>| <font color="#00dd00">✔</font> 
Caps + Ctrl + Key   | <font color="#dd0000">✘</font>     | <font color="#00dd00">✔</font>| <font color="#dd0000">✘</font>（按键不便未添加） 
TabScript           | TabScript     | TabSnippet| TabScript 
WinBind             | <font color="#00dd00">✔</font>     | <font color="#00dd00">✔</font>| <font color="#00dd00">✔</font> 
QBar                | <font color="#00dd00">✔</font>     | <font color="#dd0000">✘</font> | <font color="#00dd00">✔</font>（原作者4月最新版） 
TransplatePanel     | <font color="#00dd00">✔</font>     | <font color="#00dd00">✔</font>| <font color="#00dd00">✔</font> （增加谷歌翻译国内版） 
DAAS                | <font color="#dd0000">✘</font>     | <font color="#00dd00">✔</font>| <font color="#dd0000">✘</font>（个人用处不大未添加） 



## 按键说明 ##

如布局图片挂了可查看complete文件夹内图片，或者用浏览器查看hotkey_layout.html文件。

#### 1. Caps + Key ####
>以下省略了CapsLock键，默认是要加上的，未设置功能键的可自行设置。

![d6Dg6P.png](https://s1.ax1x.com/2020/08/25/d6Dg6P.png)

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

![d6rwj0.png](https://s1.ax1x.com/2020/08/25/d6rwj0.png)

**2.1 CapsLock + Alt + 鼠标**（临时改变鼠标速度，并在松开后复原，默认是3，范围是1~20。用于精细化操作，如：截图、取色等）

按键| 功能说明
:-:| :-:
鼠标左键|✘
鼠标中键|✘
鼠标右键|✘
鼠标滚轮向前|加快按下 Capslock+LAlt 时鼠标的速度
鼠标滚轮向后|降低按下 Capslock+LAlt 时鼠标的速度

#### 3. Caps + Shift + Key
>以下省略了CapsLock + Shift键，默认是要加上的，未设置功能键的可自行设置。

![d6sXi4.png](https://s1.ax1x.com/2020/08/25/d6sXi4.png)

**3.1 CapsLock + Shift + 鼠标**

按键| 功能说明
:-:| :-:
鼠标左键|双显示器有效，将当前软件移动到另外显示器
鼠标中键|✘
鼠标右键|✘
鼠标滚轮向前|✘
鼠标滚轮向后|✘

<br><br>

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
>
>### 命令
>
>| 命令                                                         | 功能                                                         | 说明                                                         |
>| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
>| `cl about`                                                   | 查看版本信息                                                 |                                                              |
>| `cl set`                                                     | 打开`Capslock+settings.ini`文件和`Capslock+settingsDemo.ini`文件 | `Capslock+settings.ini`各字段作用：`Global`：全局设置`QSearch`：设置搜索命令`QWeb`：设置打开网页`QRun`：设置启动程序`QStyle`：设置`+Q`输入框的样式`TabHotString`：设置`+Tab`热字串*更具体的说明请查看`CapsLock+settingsDemo.ini`文件 |
>| `ooo -> xxx`                                                 | 在`Capslock+settings.ini`以下的某字段添加一行： `ooo=xxx`如果是搜索网址： `[QSearch]`如果是文件路径： `[QRun]`如果是网址[1]： `[QWeb]`都不是： `[TabHotString]` | 例如输入`mdn -> developer.mozilla.org`，记录完成后就可以在`+Q`输入`mdn`来打开`developer.mozilla.org`如果文件是快捷方式，会自动找到快捷方式所指向的文件的路径来记录如果所记录的字符串格式类似文件路径或者网址[1]，例如`com.com.com`，就会被记录到`QWeb`，要将这类字符串记录到`[TabHotString]`，可以用`->string`命令，它会把字符串记录到`TabHotString`； 同样，`->search`会记录到`QSearch`；`->run`会记录到`QRun`；`->web`会记录到`QWeb`。*更具体的说明请查看`CapsLock+settingsDemo.ini`文件[1]: 只有以`http://`或`https://`或`www.`开头，或者包含`.com`或`.net`或`.org`的字符串才会被认为是网址 |
>| `ooo ->search xxx``ooo ->run xxx``ooo ->web xxx``ooo ->str xxx` | 在Capslock+settings.ini下的`[QSearch]` / `[QRun]` /`[QWeb]` / `[TabHotString]`字段添加一行： `ooo=xxx` | 记录完成后可以在`+Q`输入`ooo`来搜索 / 打开路径为`xxx`的文件（夹） / 网址 / 使用`+Tab`的热字串功能*更具体的说明请查看`CapsLock+settingsDemo.ini`文件 |
>| `web xxx`                                                    | 打开xxx网址                                                  | 如果`xxx`以`http://`或`https://`或`www.`开头，或者包含`.com`或`.net`或`.org`，`web`命令可以省略。例如：`google.com` |
>| `s xxx``bd xxx`                                              | 百度搜索`xxx`                                                | 百度是默认搜索引擎，即可以省略命令直接输入关键词进行搜索，除非关键词中包含其他的命令关键词可以在`Capslock+settings.ini`文件中修改默认搜索引擎，以及修改或添加搜索命令以支持其他搜索引擎。* 更具体的说明请查看`CapsLock+settingsDemo.ini`文件 |
>| `g xxx``gg xxx`                                              | 谷歌搜索`xxx`                                                |                                                              |
>| `m xxx`                                                      | MDN搜索`xxx`                                                 |                                                              |
>| `wk xxx`                                                     | 维基搜索`xxx`                                                |                                                              |
>| `tb xxx`                                                     | 淘宝搜索`xxx`                                                |                                                              |
>| `aa bb`                                                      | 用`aa`打开`bb`                                               | `aa`：`[QRun]`上有记录的一个程序`bb`：`[QRun] / [QWeb]`上有记录的一个文件（夹） / 网址简写，或具体的文件（夹）路径 / 网址例如： `[Qrun]`下记录了`ie=C:\Program Files\Internet Explorer\iexplore.exe` `[QWeb]`记录了`clp=http://cjkis.me/capslock+/` 那`ie clp`就可以用`ie`来打开`http://cjkis.me/capslock+/` 也可以直接`ie cjkis.me/capslock+` |
>| `xxx`                                                        | 如果`[QRun]`或`[QWeb]`内有记录则运行对应文件或打开对应网址如果是文件（夹）路径，打开该文件（夹）如果是网址[1]，打开该网址不是以上情况的话，百度[2] |                                                              |
>| 能根据输入，展示`[QRun]`和`[QWeb]`的记录，或输入的路径下的文件（夹）[3]可以使用通配符`?`和`*`来匹配任意一个 / 多个字符，例如： `?at`可以匹配 `bat`, `cat`, `fat`... `g*d`可以匹配 `god`, `good`, `gold`...无提示列表的情况下`Tab`展开提示列表（如果`QRun`或`QWeb`有记录的话）有提示列表的情况下，如果有选中某文件名，`Tab`可以将选中的文件名放到输入框，否则，会将第一个文件名放到输入框在展示路径下的文件时，`\`键（或`/`[4]）可以将文件（夹）名填入输入框，`Capslock+-`可以回到上级目录，`Capslock+=`可以前进到下一层目录如果要搜索类似网址的关键字，请带上搜索命令，如`s com.com`，否则将被当成网址打开`Capslock+settings.ini`中，提供给`Qbar`使用的段名`[QSearch],[QRun],[QWeb]`，支持在键名后加上`<xxx>`来作为提示，它们不会影响命令的使用。例如： `[QWeb]`下有`cx <capslox>=capslox.com`，那么`QBar`下输入`cx`打开`capslox.com``[QRun]`下需要为程序添加启动参数或以管理员权限打开的话，程序路径要用引号引起来，然后在这部分的左边加上`*RunAs`以管理员权限打开，在这部分的右边加上启动参数。例如： `ie=*RunAs "C:\Program Files\Internet Explorer\iexplore.exe" -k` *具体参照`Capslock+SettingsDemo.ini``Ctrl+Enter`会在输入的字符串前后加上`www.``.com`，并当成网址打开。例如： 输入`capslox`->`Ctrl+Enter`->打开`www.capslox.com`Qbar 支持搜索全部已安装程序，如果在启动 Capslock+ 后有安装 / 卸载程序，需要重载 Capslock+ 。[1]: 只有以`http://`或`https://`或`www.`开头，或者包含`.com`或`.net`或`.org`的字符串才会被认为是网址。否则，请在网址前面加上命令`web`。[2]: 通过修改`Capslock+settings.ini`文件下，`[QSearch]`段的`default`可以设置默认搜索[3]: 在展示输入的路径下的文件时，为了保证加载速度，在文件过多的时候，会放弃加载部分文件的图标，直接使用一个`空白文件`样式的图标[4]: `\`键在文件路径输入时会频繁使用，而`\`键实在太远了，所以特地让`/`键也实现和`\`键一样的功能，如果需要输出`/`符号可以用`Capslock+/` | 左侧排版问题不想改了，自行参考 [原文档](https://capslox.com/capslock-plus/#clTabScript) |                                                              |



## 补充说明

请查看原文档 [补充说明](https://capslox.com/capslock-plus/#补充说明)



## 如何自行设置全局的按键

>在CapsLock+settings.ini里[Keys]设置，请对照CapsLock+settingsDemo.ini 来配置相关设置，里面说的很详细

<br>

参考资料：[AutoHotkey官方文档](https://www.autohotkey.com/docs/AutoHotkey.htm)
