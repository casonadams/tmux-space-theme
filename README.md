# tmux-space-theme
tmux theme inspired by SpaceVim

# Setup
## Linux
Install a powerline font and use it with terminal
[DejaVu Sans Mono](https://github.com/powerline/fonts/blob/master/DejaVuSansMono/DejaVu%20Sans%20Mono%20for%20Powerline.ttf).

I prefer alacritty update this line in the `~/.config/alacritty/alacritty.yml` file

```bash
family: "DejaVu Sans Mono for Powerline"
```

### Install gitmux for git info in status bar
```bash
sudo curl -L https://github.com/arl/gitmux/releases/download/v0.4.1/gitmux_0.4.1_linux_amd64.tar.gz | tar xC /usr/local/bin/
```

## OSX
Install a powerline font and use it with terminal
[Source Code Pro](https://github.com/powerline/fonts/blob/master/SourceCodePro/Source%20Code%20Pro%20for%20Powerline.otf).

I prefer alacritty update this line in the `~/.alacritty.yml` file

```bash
family: "Source Code Pro for Powerline"
```

### Install gitmux for git info in status bar
```bash
sudo curl -L https://github.com/arl/gitmux/releases/download/v0.4.1/gitmux_0.4.1_macOS_amd64.tar.gz | tar xC /usr/local/bin/
```

## Config file
Add `set -g @plugin 'casonadams/tmux-space-theme'` to tmux.conf file then install plugin `ctrl+b I`

```bash
if "test ! -d ~/.tmux/plugins/tpm" \
     "run 'git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm && ~/.tmux/plugins/tpm/bin/install_plugins'"

set -g @plugin 'casonadams/tmux-space-theme'

run -b '~/.tmux/plugins/tpm/tpm'
```

## Options
Add `setw -q @show-full-window-path true` to tmux.conf file to show full path in window.

# Special Thanks
https://github.com/arl/gitmux
https://github.com/egel/tmux-gruvbox
