这是i3wm的配置文件
## i3wm美化教程

### 简介

i3wm是一款稳定高效的平铺式窗口管理器,  本脚本可以一键将i3wm配置为Screenshots中的样式, 并且可以选择是否同时配置vim, ranger或zsh

* 本脚本同时附带一些壁纸
* 本脚本同时附带触摸板设置, 包括启用轻触, 多指操作等功能
* 依赖项:

  ```
  xfce4-screensaver xfce4-power-manager i3-gaps conky copyq dunst blueman kitty ranger rofi polybar ccal lunar-date xbindkeys brightnessctl i3lock-fancy-git neofetch ranger vim(可选)  zsh(可选)
  ```

* 推荐安装(脚本不自带, 需自行安装)

  ```
  keynav warpd
  ```

### 注意事项

* polybar天气插件(位于`~/.config/i3/polybar/script/weather-bar.sh`)中地区需要自行更改, 默认值为哈尔滨
* 本脚本不会更改默认shell,  如果您选择安装了zsh配置文件, 而目前使用的不是zsh, 需要手动使用chsh命令将默认shell更改为zsh
* 可选配置文件(zsh, vim, ranger)需要自行提前安装对应的软件包
* 安装有两种方式, 一种是复制文件到对应目录, 一种是创建软连接到对应目录
  * 如果选择复制方式, 在安装成功后可以删除或移动此目录, 如果选择链接方式, 安装成功后不可删除或移动此目录
  * 如果选择链接方式, 务必把该目录放到主目录下, 不能改名, 否则会失效
  * 如果选择链接方式, 桌面背景和存放rofi相关脚本的bin目录仍会以复制的方式安装,  因为用链接方式安装这些项目无效

  ### 安装

执行：

```bash
./install.sh
```

安装完成后，如果你已经安装了vim配置文件，请记得在第一次启动vim时运行:PlugInstall

github: https://github.com/wiwyil2tr/My_i3wm_theme_configure

