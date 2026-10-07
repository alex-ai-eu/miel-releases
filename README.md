# Miel releases

Alpha builds of [Miel](https://getmiel.io/), an office suite that keeps its
data encrypted on the device, and the feed its updater reads. Miel's source
is not published here; this repository only holds what is released.

## Installing

Miel runs on Macs with Apple silicon and macOS 14 or later.

```sh
brew install alex-ai-eu/tap/miel
```

The first time Miel opens, macOS refuses because the alpha is not notarized
by Apple yet: choose **System Settings > Privacy & Security > Open Anyway**.

## Updating

Miel updates itself: choose **Miel > Check for Updates…**, or turn on daily
checks in **Settings > General**. Each update is signed with Miel's update
key and checked before it is installed.

## What each release holds

- `Miel-<version>.dmg`: the app.
- `appcast.xml`: the signed update feed, read through
  `https://getmiel.io/appcast.xml`.

Releases are made by `cargo xtask publish` in the Miel repository; do not
edit or upload them by hand.
