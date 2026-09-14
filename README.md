# LiveWallet

**Learn bitcoin by *using* bitcoin.**

Build a wallet from scratch, in a notebook, and understand every line.

LiveWallet is a set of [Livebook](https://livebook.dev) notebooks for BSV.
You write real Elixir, handle real keys, and move real bitcoin.
It is the hands-on companion to [Bitcoin: An Introduction](https://livewallet.app/bitcoin-book), which covers the why.

[![](https://github.com/afomi/livewallet-site/blob/main/assets/images/livewallet-screenshot.png?raw=true)](https://www.livewallet.app)

## Important notice

Run LiveWallet on your own machine or on a server you trust.
The notebooks handle private keys that control bitcoin.
LiveWallet is experimental software for education.
Use at your own risk, and keep amounts under 1 USD.

## How to use it

[![Run in Livebook](https://livebook.dev/badge/v1/blue.svg)](https://livebook.dev/run?url=https%3A%2F%2Fraw.githubusercontent.com%2Fafomi%2Flivewallet%2Fmain%2Fstart-here.livemd)

1. Install [Livebook](https://livebook.dev).
   The desktop app is a normal download for Mac, Windows and Linux, from [livebook.dev/#install](https://livebook.dev/#install).
2. Click the badge above, or open [start-here.livemd](start-here.livemd) from a clone of this repo.
   It has a map of every notebook and which ones to do first.
   The [table of contents](table-of-contents.livemd) lists them all in one place.
3. Everything starts on testnet, where coins have no value.
   When you want real bitcoin, add a Livebook secret named `LB_NETWORK` with the value `main`.
   Every notebook shows a banner saying which network you are on.
4. Run a notebook top to bottom.
   Each ends with a Review cell that prints `PASS` when you did what the notebook set out to do.

There is no numbered order.
Each notebook says at the top what to do before it, and the map shows those as arrows.

## Layout

| Directory | What is in it |
|---|---|
| `wallet/` | Seed phrases, keys, addresses, derivation paths, the key hierarchy |
| `transactions/` | Receive, verify, send, and time-locked transactions |
| `tokens/` | Inscriptions, on-chain posts, and recovering assets from old keys (in progress) |
| `governance/` | Multisig ceremonies and a function-shaped wallet |
| `tools/` | Utility notebooks that are not lessons |
| `docs/` | Specs and reference material; `docs/CONCEPTS.md` is the vocabulary |

`PLAN.md` is the backlog.
`check.exs` checks the repo's links, fences and map; run it with `elixir check.exs`.

## Related

* [Bitcoin: An Introduction](https://livewallet.app/bitcoin-book), the companion book
* [Bitcoin whitepaper](https://bitcoin.org/bitcoin.pdf)
* [bsv-ex](https://github.com/libitx/bsv-ex), the Elixir library used for keys, scripts and transactions

[Feedback welcome](https://github.com/afomi/livewallet/issues/new)
