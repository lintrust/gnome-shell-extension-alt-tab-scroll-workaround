# May be the best solution until now for users who meet scrolling bug on Ubuntu when using Chrome core apps like vscode, Electron, Chrome, Edge:
This bug is exists for about 2 years.
This bug is described in several open issues:
- Editor: scroll jumps randomly (related to Chrome, Electron, xinput) #28795 https://github.com/Microsoft/vscode/issues/28795
- When used with Chrome on Ubuntu, the scroll wheel functions abnormally #184260 https://github.com/microsoft/vscode/issues/184260
- Buggy scrolling in VSCode/Chrome/Electron apps? https://www.reddit.com/r/pop_os/comments/v2d1na/buggy_scrolling_in_vscodechromeelectron_apps/?rdt=33348
- Electron scroll erratic jumping https://coldnorthadmin.com/posts/electron_scroll/
- VSCode editor window intermittently jumps to bottom when rolling mouse scroll wheel https://stackoverflow.com/questions/68331851/vscode-editor-window-intermittently-jumps-to-bottom-when-rolling-mouse-scroll-wh
- Jumpy scrolling between chromium and VS Code https://bbs.archlinux.org/viewtopic.php?id=277469
- Ubuntu 18.04 inconsistent scrolling behavior https://askubuntu.com/questions/1209490/ubuntu-18-04-inconsistent-scrolling-behavior
- Fixing Mouse Wheel on Chrome in Ubuntu 18.04 Virtualbox / VMWare https://dev.to/danvoyce/fixing-mouse-wheel-on-chrome-in-ubuntu-18-04-virtualbox-vmware-143n
- https://github.com/pop-os/pop/issues/2331
- https://github.com/atom/atom/issues/15482
- GitLab: [GNOME/mutter#401](https://gitlab.gnome.org/GNOME/mutter/-/issues/401)
- Chromium: [chromium#608246](https://bugs.chromium.org/p/chromium/issues/detail?id=608246)
- Chromium: [chromium#807187](https://bugs.chromium.org/p/chromium/issues/detail?id=807187)
- Ubuntu 18.04环境下 VS Code 鼠标滚动异常问题 https://www.jianshu.com/p/0e88407bffc1
- https://www.google.com/search?q=why+vscode+scroll+with+chrome+on+ubuntu 




I do nothing but found this solution for myself and fork it to here, wish helping who meet the same bug. 
-----------------------------------

# As who said in github issue comment, "Install it then you'r Golden".
# GNOME Shell Extension Alt+Tab Scroll Workaround

> Quick fix to the bug where scrolling in one application is repeated in another when switching between them using `Alt+Tab` (e.g., VS Code and Chrome)

As an example, after scrolling VS Code and switching to Chrome using `Alt+Tab` or `Super+Tab`, the VS Code scroll would be repeated in Chrome. Installing the extension should avoid this.

This bug is described in several open issues:
- https://github.com/Microsoft/vscode/issues/28795
- https://github.com/pop-os/pop/issues/2331
- https://github.com/atom/atom/issues/15482
- GitLab: [GNOME/mutter#401](https://gitlab.gnome.org/GNOME/mutter/-/issues/401)
- Chromium: [chromium#608246](https://bugs.chromium.org/p/chromium/issues/detail?id=608246)
- Chromium: [chromium#807187](https://bugs.chromium.org/p/chromium/issues/detail?id=807187)

## Usage

### Installation from GNOME Extensions

The extension can be found at the GNOME Extensions website: [Alt+Tab Scroll Workaround](https://extensions.gnome.org/extension/5282/alttab-scroll-workaround/). Just open the page, turn the extension on, and you're ready to go.

### Installation from GitHub

If, instead, you prefer to install it from this repository, follow the next steps.

Clone and enter the repository:
```
git clone https://github.com/lucasresck/gnome-shell-extension-alt-tab-scroll-workaround.git
cd gnome-shell-extension-alt-tab-scroll-workaround
```

Install the extension:
```
make install
```

Restart the GNOME Shell:

- Press `Alt+F2`;
- Type `r` and press `Enter`.

> At this point, the extension should be enabled. If not:
> ```
> make enable
> ```

## License
GPLv3
