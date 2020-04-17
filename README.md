# Better Development Environment

A collection of tools, configs, etc. to setup new development environments in Linux.

Each time I start working on a new Linux machine, I end up installing the same things, finding solutions for the same problems, and just generally wasting time doing things that I've done before.

This README (and potentially bash scripts) simplify the first-time installation and setup of a powerful Linux development environment.

## Ubuntu

.. note:: The following instructions assume that you are running Ubuntu 18.04. None of the following instructions have been tested on other Ubuntu versions.

### Zsh

Configurations, tools, themes, etc. assume that you are using `zsh` instead of a vanilla `bash` shell.

Install `zsh` and make it the default shell for Ubuntu.

```bash
sudo apt install -y zsh
chsh -s /bin/zsh
```

After installing, it is recommended that you reboot.

### Make Zsh Pretty
I hate Ubuntu's default color scheme and the terminal is painful to look at out of the box. This section goes over some tools to make terminal better to use and look at.

#### Install Powerlevel10k

[Powerlevel10k](https://github.com/romkatv/powerlevel10k) is a theme for `Zsh`.

Install from source.

```bash
git clone --depth=1 https://github.com/romkatv/powerlevel10k
echo 'source ~/powerlevel10k/powerlevel10k.zsh-theme' >>! ~/.zshrc
```

Configure and setup by resourcing zshrc.

```bash
source ~/.zshrc
```

#### Install Fonts (Optional)

Follow the instructions on the powerlevel10k README to [install better fonts](https://github.com/romkatv/powerlevel10k#meslo-nerd-font-patched-for-powerlevel10k).

### Other Tools

Tmux is a terminal multiplexer. Effectively, it allows you to split a single terminal session into multiple panes with multiple sessions.

Ranter is a file explorer

Htop is a more powerful resource utilization visualizer.

```bash
sudo apt install -y tmux ranger htop
```


```bash
```
