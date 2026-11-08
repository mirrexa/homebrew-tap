# Swarmfile Homebrew tap

Homebrew tap for [Swarmfile](https://swarmfile.com) — a cloud-streamed virtual
filesystem for teams working with very large files.

## Install

```sh
brew tap mirrexa/tap
brew install --cask swarmfile
```

## Update

Swarmfile updates itself in place (the desktop app has a built-in updater), so
you normally don't need `brew upgrade`. The cask is marked `auto_updates true`
for that reason. To reinstall or pin a specific version, use the standard cask
commands.

## Uninstall

```sh
brew uninstall --cask swarmfile
# to also remove app data:
brew uninstall --zap --cask swarmfile
```

## What gets installed

The cask installs the notarized universal `.pkg` from
`releases.swarmfile.com`. It bundles the mount helper (FUSE-T, kext-free), the
engine, the tray app, and their LaunchAgents — no separate macFUSE install is
required.
