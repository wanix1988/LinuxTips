# ubuntu系统配置相关

1. ubuntu16.04启动进入文本模式
    > sudo vi /etc/default/grub
    >> 
       GRUB_CMDLINE_LINUX_DEFAULT="quiet splash text"
       GRUB_CMDLINE_LINUX="text"
       GRUB_TERMINAL=console
    > sudo update-grub
    
    > sudo systemctl set-default multi-user.target
