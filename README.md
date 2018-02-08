# tmux-conf
my zsh env

1, 首先需要安装 oh-my-zsh，然后增加 plugin 配置和最后的个性化设置
2, 将tmux 配置文件copy 为 `~/.tmux.conf`。通过[tmp](https://github.com/tmux-plugins/tpm)安装需要的插件

### 注意事项

- vim 在 tmux 中样式各种不协调。通过安装[powerline-fonts](https://github.com/powerline/fonts)可以解决
具体可以查看我的 [vimrc 配置](https://github.com/boyaziqi/vimrc_config)

- zshrc 里 plugins 选项中的 vi-mode 和 history-substring-search 顺序不能颠倒，不然 vi-mode 方向键不能正确搜索历史命令
