# AutoSEU

[![Release Version](https://img.shields.io/github/release/TimeLeSsROMO/AutoSEU)](https://github.com/TimeLeSsROMO/AutoSEU/releases/)

自动进行东南大学的每日健康申报以及次日的出校审批

一个自动每日健康申报以及次日出校审批的python脚本，基于Python-Selenium，Chrome-Chromedriver

基于[StephenHoo/AutoLogin](https://github.com/StephenHoo/AutoLogin)，但是分支不过去，是我自己太憨了…只能自己新建一个项目了，请谅解。部分内容可以参见这位老哥的内容，普通使用只需要在这里下载，点开即可。

如果您想自己编译python代码，则需要：

python3

安装selenium库

与浏览器对应的Webdriver

正常使用请前往[Releases](https://github.com/TimeLeSsROMO/AutoSEU/releases/tag/AutoSEU_1.6)下载最新版本安装包并解压，确保文件夹中的chromedriver.exe与AutoSEU_1.6.exe在同一文件夹即可（chromedriver需要与chrome浏览器版本对应，压缩包中自带的是目前的最新版，如有更新请自行前往[对应网站](http://npm.taobao.org/mirrors/chromedriver)下载）。
直接点击exe文件运行程序，第一次运行需要输入您的一卡通号、密码、家长、辅导员等信息（完全保存个人计算机本地，并不会泄露给任何人），之后不需要再进行此操作。

需要安装好chrome浏览器，最好是安装在默认位置，否则操作会比较麻烦

请确保在现版系统中进行过至少一次健康申报和出校审批，否则可能出现奇怪的错误导致无法正常运行

Version 1.6更新日志：

1.重写了60%以上的代码（很谨慎的描述），精简部分无用代码，各功能在目前的新版网站上完美运行

2.新增更多人性化选项，可以单独进行健康申报或者出校审批

3.新增检测是否处在健康申报和出校审批的时间段功能

4.新增出校审批是否通过的检测，完善检测是否已经进行健康申报的逻辑

5.新增销假功能，用于顺利进行出校审批（2天前新改版的内容，无语）

6.完善每日体温参数；可自定义请假理由

7.完善申报失败，网站故障时的提醒功能（东大的网站稳定性真的呵呵）

8.增加更多提醒内容，增加易用性

Tips：

校区仅支持丁家桥校区，毕竟之前其他校区的老哥们也是这么搞的，只支持自己校区~其他校区可联系我进行修改

为啥直接叫1.6，因为觉得好听~而且之前漏洞比较大（判断是否进行健康申报的逻辑是看有没有新增按钮……不应该是检查新增申报的日期吗。。放心，类似的都改了）；代码比较乱，很多无用和冗余的内容；憨憨学校网页改版太大，之前的基本都废了。So，1.3 to 1.6应该不过分吧
