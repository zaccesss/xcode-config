# Contributing

Thanks for taking an interest. Contributions are welcome: preference fixes, install script fixes
and guide improvements.

## What belongs here

- A key in `prefs.txt` that Xcode reads differently from what
  [guides/reference.md](guides/reference.md) says
- An install script bug: a file it copies to the wrong place, a value it writes with the wrong type
  or a second run that changes something
- A path or step that is wrong for a current Xcode release
- Improvements to the guides

## What does not belong here

- A preference that only reflects one person's taste rather than something broadly useful, keep
  that in your own copy
- Theme colours, which are generated in [Zacess Themes](https://github.com/zacesshq/themes)

## How to contribute

1. Fork the repository and create a branch named `fix/<short-description>` or
   `feat/<short-description>`.
2. Change values in `prefs.txt` only, never in the script.
3. Run `bash -n apply.sh` and `shellcheck apply.sh`, then run `./apply.sh` with Xcode closed and
   confirm a second run prints `Xcode matches the recorded setup.`
4. Open a pull request with a clear title and a one-paragraph description of what changed and
   why. CI checks `prefs.txt`, the key bindings file and the script.

## Reporting bugs

Open an issue with your Xcode version, your macOS version and the install script's output, what you
expected versus what happened.

More about me and my work: [isaacadjei.me](https://isaacadjei.me).
