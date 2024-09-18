# stress-ng-snap

This is a snap packaging of [stress-ng](https://github.com/ColinIanKing/stress-ng), a tool to load and stress a computer.

## Install

This snap is available under [developer mode confinement](https://snapcraft.io/docs/install-modes#heading--devmode).
This is because `stress-ng` is a testing tool that needs a wide range of access to the system.
Keep in mind that snaps installed in developer mode don't upgrade automatically like [strictly confined and classic snaps](https://snapcraft.io/docs/snap-confinement).
The snap should be removed after testing or [updated manually](#update).

Because of its confinement mode, this snap is only available in the `latest/beta` and `latest/edge` [channels](https://snapcraft.io/docs/channels).
The most stable revision can be installed with:
```bash
sudo snap install stress-ng-dev --devmode --beta
```

## Update


To manually update the snap, use:

```bash
sudo snap refresh stress-ng-dev --devmode
```

## Use

For usage instructions refer to:

- [Ubuntu Wiki page about stress-ng](https://wiki.ubuntu.com/Kernel/Reference/stress-ng)
- [Ubuntu Man page](https://manpages.ubuntu.com/manpages/noble/man1/stress-ng.1.html)

### Add aliases
You can add [aliases](https://snapcraft.io/docs/commands-and-aliases) to run the program commands without the namespace. For example:
```console
$ sudo snap alias stress-ng-dev.stress-ng stress-ng
Added:
  - stress-ng-dev.stress-ng as stress-ng

$ which stress-ng
/snap/bin/stress-ng
```

### Local Build

Build it using [Snapcraft](https://snapcraft.io/snapcraft):

```bash
snapcraft -v
```

Then, install it in [devmode](https://snapcraft.io/docs/install-modes#heading--devmode):

```bash
sudo snap install --devmode *.snap
```
