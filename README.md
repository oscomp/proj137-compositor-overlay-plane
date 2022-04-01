# proj137-compositor-overlay-plane
UOS下wayland合成器支持overlay plane

### 项目描述

1. Wayland 是一个用于 混成窗口管理器 与其客户端对话的协议，也是一个实现该协议的库。 GNOME 和 KDE Plasma 等一些桌面环境支持 Wayland。 它还有一个混成器实现参考叫做 Weston。为支持多种处理器架构（x86-64、risc-v、arm64）的Linux操作系统开发一个共享库，可以指定应用程序运行时候加载此库
2. wlroots是一个基于wayland协议的合成器。
3. kwin包含kwin_x11和kwin_wayland，kwin_wayland实现了wayland协议的合成器。
4. 合成分为软件合成和硬件合成。软件合成是使用OpenGL或OpenGLES合成窗口图片后利用drm上屏显示的过程。硬件合成是客户端根据合成器提供的接口把客户端的纹理数据设置到drm的Overlay plane中去，由硬件来合成。

### 所属赛道

2021全国大学生操作系统比赛的“OS功能设计”赛道

### 参赛要求

- 以小组为单位参赛，最多三人一个小组，且小组成员是来自同一所高校的本科生（2021年春季学期或之后本科毕业的大一~大四的学生）
- 如学生参加了多个项目，参赛学生选择一个自己参加的项目参与评奖
- 请遵循“2021全国大学生操作系统比赛”的章程和技术方案要求

### 项目导师

谭芳

* github tantan580
* email tanfang@uniontech.com

### 难度

难

### 特征

* 熟悉Linux显示服务框架。
* 熟悉OpenGL，OpenGLES，Drm，wayland协议等图形技术栈。
* 熟悉C或C++语言。
* 熟悉图形学原理。

### 参考项目

* weston

### License

* [GPL-3.0-only](https://opensource.org/licenses/GPL-3.0)

## 预期目标

### 注意：下面的内容是建议内容，不要求必须全部完成。选择本项目的同学也可与导师联系，提出自己的新想法，如导师认可，可加入预期目标

### 题目一

在kwin_wayland中实现Overlay Plane功能

### 题目二

在wlroots中实现Overlay Plane功能
