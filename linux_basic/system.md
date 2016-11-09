# 系统相关操作

1. 停止关机
    > shutdown -c
    > 如果已经开始关机，那么有可能来不及，可以尝试使用pkill shutdown

2. 特定的时间运行Linux命令
    > at 
    > 如：  > at 10:38 PM Fri

            at>  cowsay 'hello'
            at> CTRL + D

3. 杀死挂起进程的简单方法
    > xkill, 然后选择要杀死的窗口
    > 如果整个系统挂掉了，那就按住alt+sysrq，然后输入REISUB

4. man手册设置
    > export PAGER=most
    >> 你需要安装 ‘most’；她会使你的你的man手册的色彩更加绚丽。

    > export MANWIDTH=80
    >>  你可以用这个命令给man手册设定指定的行长

    > man -H <command>
    >> 可以使用-H在默认浏览器中打开任意的man页。
    >>> 注意啦，以上的命令只有在你将默认的浏览器设置到环境变量$BROWSER中了之后才效果哟。

5. 设置文本模式下显示中文/输入中文
    > [Linux text mode display / input Chinese](http://prog3.com/sbdm/blog/frombegintoend/article/details/7973257)
    >> 仅验证了使用fbterm显示中文部分，输入未使用

6. 文本模式下字体和大小设置
    > sudo dpkg-reconfigure console-setup
