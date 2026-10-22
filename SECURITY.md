# Security Policy

## Scope

This repository is IDE configuration: a preferences list, colour themes, a key bindings file, one
small install script and guides. It contains no service and no library. In scope:

- An install script that writes outside `~/Library/Developer/Xcode/UserData` and the
  `com.apple.dt.Xcode` domain, follows a crafted path somewhere unexpected or runs a line of
  `prefs.txt` as code
- A setup instruction that would leave insecure file permissions behind

## Out of scope

- A vulnerability in Xcode itself or in the WakaTime app, report that upstream

## Reporting a vulnerability

> [!IMPORTANT]
> Report privately, not in a public issue. Email contact@isaacadjei.me with details and
> reproduction steps. Expect an acknowledgement within a few days.
