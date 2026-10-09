# WG Signing Test

A sandbox for testing how a signed `.pyc` is delivered by `git push`. It is not a mod and is not
meant to be installed.

## Layout

The same as every v2 mod repo:

```
PnFModsLoader.py
PnFMods/
  TestMod/
    Main.pyc        <- the signed file goes here
```

## Delivering

1. Clone this repo.
2. Put the signed file at `PnFMods/TestMod/Main.pyc`.
3. Commit and push to `main`.

In a real mod repo the path is `PnFMods/<the mod's folder>/Main.pyc`, plus one `.pyc` for every
other `.py` the mod has. Only `.pyc` files are delivered; the `.py` source never goes in a public
repo.

Nothing checks a push here yet.
