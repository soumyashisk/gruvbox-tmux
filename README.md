<h1 align="center">Gruvbox for Tmux</h1>

<p align="center">
  A warm and retro Gruvbox theme for <a href="https://github.com/tmux/tmux">Tmux</a>
</p>

<p align="center">
  <em>Based on <a href="https://github.com/catppuccin/tmux">Catppuccin Tmux</a></em>
</p>

<p align="center">
  <img src="./preview.png" alt="Gruvbox Tmux Preview"/>
</p>

## About

This Tmux theme brings the beloved Gruvbox color scheme to your terminal multiplexer. With its warm, earthy tones and excellent contrast, Gruvbox provides a comfortable and aesthetically pleasing environment for your terminal sessions.

## Installation

### TPM (Recommended)

1. Install [TPM](https://github.com/tmux-plugins/tpm)
2. Add the Gruvbox plugin to your `~/.tmux.conf`:

```bash
set -g @plugin 'gruvbox-tmux'
# ...alongside
set -g @plugin 'tmux-plugins/tpm'
```

3. Press `prefix + I` to install the plugin

### Manual Installation

1. Copy the theme configuration from [gruvbox.tmuxtheme](./gruvbox.tmuxtheme) into your Tmux config (usually stored at `~/.tmux.conf`)
2. Reload Tmux by either restarting the session or reloading it with `tmux source-file ~/.tmux.conf`

## Configuration

The theme supports various customization options to match your preferences.

> **Note:** To display icons correctly, please use a [Nerd Font](https://www.nerdfonts.com/) patched font.

##### Enable window tabs

By default, the theme places the `window-status` in the `status-right`. With
`@gruvbox_window_tabs` set to `on`, the theme will place the
directory within the `status-right` and move the window names to the
`window-status` format variables.

```sh
set -g @gruvbox_window_tabs on # or off to disable window_tabs
```

##### Configure separator

By default, the theme will use a round separator for left and right.
To overwrite it use `@gruvbox_left_separator` and `@gruvbox_right_separator`

```sh
set -g @gruvbox_left_separator ""
set -g @gruvbox_right_separator ""
```

##### Enable DateTime

By default, the `date_time` componenet is set to off.
It can be enabled by specifing any tmux date and time format.

```sh
set -g @gruvbox_date_time "%Y-%m-%d %H:%M"
```

##### Enable User

By default, the `user` componenet is set to off.
It can be enabled by toggoling it on.

```sh
set -g @gruvbox_user "on"
```

##### Enable Host

By default, the `host` componenet is set to off.
It can be enabled by toggoling it on.

```sh
set -g @gruvbox_host "on"
```

[style-guide]: https://github.com/catppuccin/catppuccin/blob/main/docs/style-guide.md

## 💝 Thanks to

- [Pocco81](https://github.com/catppuccin)
- [vinnyA3](https://github.com/vinnyA3)
- [rogeruiz](https://github.com/rogeruiz)

&nbsp;

<p align="center"><img src="https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/footers/gray0_ctp_on_line.svg?sanitize=true" /></p>
<p align="center">Copyright &copy; 2021-present <a href="https://github.com/catppuccin" target="_blank">Catppuccin Org</a>
<p align="center"><a href="https://github.com/catppuccin/catppuccin/blob/main/LICENSE"><img src="https://img.shields.io/static/v1.svg?style=for-the-badge&label=License&message=MIT&logoColor=d9e0ee&colorA=363a4f&colorB=b7bdf8"/></a></p>
