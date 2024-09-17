# stress-ng-snap

This is a snap packaging of [stress-ng](https://github.com/ColinIanKing/stress-ng), a tool to load and stress a computer.

## Install

Because `stress-ng` is a test tool that needs a wide access to the system this snap is available under [devmode confinement](https://snapcraft.io/docs/install-modes#heading--devmode) only.

```bash
sudo snap install stress-ng --devmode
```
## Use

For usage instructions refer to:

- [Ubuntu Wiki page about stress-ng](https://wiki.ubuntu.com/Kernel/Reference/stress-ng)
- [Ubuntu Man page](https://manpages.ubuntu.com/manpages/noble/man1/stress-ng.1.html)


### Local Build

Firstly, build it using [Snapcraft](https://snapcraft.io/snapcraft):

```bash
snapcraft -v
```

Then, install it in [devmode](https://snapcraft.io/docs/install-modes#heading--devmode):

```bash
sudo snap install --devmode *.snap
