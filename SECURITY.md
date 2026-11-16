# Security policy

Hundo runs game modules written by anyone, so their sandbox is what matters
most: a module must not read files beyond the save it is given, reach the
network, or run anything on the machine.

## Reporting a vulnerability

Report it privately, never in a public issue:
[open a security advisory](https://github.com/hundo-app/releases/security/advisories/new)
(on `hundo-app/modules` for something in the SDK, the contract or a module).

Say what is affected, how to reproduce it, and what it allows. You will get an
answer within a week. Once fixed, the advisory is published with credit to
you, unless you prefer otherwise.

## Supported versions

Only the latest release receives fixes; the app updates itself (or through
Flathub, or your package manager).

## In scope

- escaping a module's sandbox (files, network, environment, host memory)
- installing or updating a module or the app without a valid signature
- a module's report or a game's files making the app open or run something
- the app sending anything off the machine without the reader allowing it
