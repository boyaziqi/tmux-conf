# my zsh env conf

我的 zsh 环境配置, 包括 oh-my-zsh, tmux, vi

### 使用

1, 首先需要安装 oh-my-zsh，然后增加 plugins 配置和最后的个性化设置

2, 将tmux 配置文件copy 为 `~/.tmux.conf`。通过[tmp](https://github.com/tmux-plugins/tpm)安装需要的插件
```shell
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
```

### 注意事项

- vim 在 tmux 中样式各种不协调。通过安装[powerline-fonts](https://github.com/powerline/fonts)可以解决
具体可以查看我的 [vimrc 配置](https://github.com/boyaziqi/vimrc_config)

- zshrc 里 plugins 选项中的 vi-mode 和 history-substring-search 顺序不能颠倒，不然 vi 模式 方向键不能正确搜索历史命令

- tmux 可能无法共享系统剪贴板，如果使用item，勾选上`Applications in terminal may access clipboard`即可。如果通过
    `reattach-to-user-namespace` 解决，需要首先安装，然后在取消相应行注释。不然启动会报错。macos 执行如下命令安装：
```shell
    brew install reattach-to-user-namespace
```
