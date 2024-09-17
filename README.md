# stress-ng-snap

This is a snap packaging of [stress-ng](https://github.com/ColinIanKing/stress-ng), a tool to load and stress a computer.

## Install

This snap is available under [developer mode confinement](https://snapcraft.io/docs/install-modes#heading--devmode).
This is because `stress-ng` is a testing tool that needs a wide range of access to the system. 
Keep in mind that snaps installed in developer mode don't upgrade automatically. 
It should be removed after testing or upgraded manually.

```bash
sudo snap install stress-ng --devmode
```
## Use

For usage instructions refer to:

- [Ubuntu Wiki page about stress-ng](https://wiki.ubuntu.com/Kernel/Reference/stress-ng)
- [Ubuntu Man page](https://manpages.ubuntu.com/manpages/noble/man1/stress-ng.1.html)


### Local Build

Build it using [Snapcraft](https://snapcraft.io/snapcraft):

```bash
snapcraft -v
```

Then, install it in [devmode](https://snapcraft.io/docs/install-modes#heading--devmode):

```bash
sudo snap install --devmode *.snap
