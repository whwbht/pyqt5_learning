入门网站：
https://doc.itprojects.cn/0001.zhishi/python.0008.pyqt5rumen/index.html#/02.ui
虚拟环境的创建，用到什么开发什么，exe文件就会减小

第一个pyqt5程序。这个是模板，相当于helloworld/基本格式
创建一个界面

以后所有需要添加的 控件，都可以直接在网上进行搜索。具体的步骤都存在


*********基本UI*********
button，创建的时候需要 指定parent，这样才能显示出来，类似的空间都需要设置parent
QLabel，文本
QLineEdit，输入框
窗口大小和位置。比如窗口中央位置、获取屏幕中心位置、数据类型打印等
窗口icon左上角图表设置/若有一些最上列不能修改，那么就删掉，剩下的完全自己设置控件即可，例如mac中的菜单栏不能修改，那么就去掉

*********布局*********
代码封装，类//因为存在很多个空间，那么类就可以很好的解决这个问题
界面的排序方式

水平布局QHBoxLayout和垂直布局QVBoxLayout/弹簧addStretch/
九宫格布局/格子grid使用/若还有其他需求，可以直接百度然后学习。

form表单布局/登陆界面的设置和使用
stacklayout抽屉布局/wechat类似/鼠标点击事件触发不同的窗口(通过抽屉布局的索引直接展示)


*********窗口*********
qwidget/之前讲的,通过控件来实现窗口,比较自由,但是啥都没有/
qmainwindow/菜单栏,状态栏,显示区域/menuBar的使用	
qdailog/对话框,弹出操作/一般不作为主窗口/可以作为鼠标点击事件后弹出该窗口

*********信号与槽*********Qt核心内容
信号signal/状态，时间/触发、绑定/
槽slot/槽函数/触发槽可以通过库函数比如click，也可以自己写信号mysignal进行触发

步骤：1信号声明/2信号与槽进行绑定/3信号触发槽函数

技术分享/云函数/非常的高效有用


*********qt designer*********相当于是一个软件了，可以设计界面/
软件设计界面/然后代码里面调用该软件名称可以直接实现界面功能/信号与曹等等/但是没法自定义槽函数
因此/设计的时候通过py代码加载ui文件，获取里面的控件信息，然后对其操作。


*********线程*********
界面的显示用主线程来操作，逻辑功能代码或耗时操作的代码用另外的线程进行处理/若只有1条线程，那么执行该线程时再点击，就会出现卡死的现象。/cpu一个线程只能干一件事
函数执行完成的时候，局部变量就清空了，所以线程在创建的时候，不要写成局部变量。

关键词：进程，线程，携程/输入输出缓存区

记住Qt的对应网站，不懂得函数、类怎么使用的可以直接搜索。官方文档的使用非常重要
