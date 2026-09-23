# Contributing to Gubernaut

This is the default guide for every repository in the organisation that does not carry its own.

## Where a change goes

| Repository | What to send it |
|---|---|
| [**gubernaut**](https://github.com/thegubernaut/gubernaut) | Every code change: the Python proxy, the JavaScript and Rust controllers, the ElizaOS plugin, the bench. Its own [CONTRIBUTING.md](https://github.com/thegubernaut/gubernaut/blob/main/CONTRIBUTING.md) has the setup and the tests |
| [**tiller**](https://github.com/thegubernaut/tiller), [**keel**](https://github.com/thegubernaut/keel) | Nothing directly. They are copies of the main repository with their own front pages, re-synced from it, so a pull request there would be overwritten. Send it to **gubernaut** instead |
| [**Gubernaut_Validation**](https://github.com/thegubernaut/Gubernaut_Validation) | Reproduction reports, errata and questions about the paper's evidence, as issues. The sealed data under `02_data/` is never edited: a correction ships as a new, separately sealed release |

## What makes a change easy to accept

- **A number needs its source.** Every published figure comes from a recorded run. A change that
  states a new one needs the receipt behind it.
- **Tests with the change.** A fix arrives with the test that would have caught it.
- **A small diff.** One idea per pull request.

Everyone here follows the [code of conduct](CODE_OF_CONDUCT.md).
