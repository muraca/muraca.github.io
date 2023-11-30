---
layout: page
title: Sketchbook
description: A collection of ideas for future blog posts.
permalink: /sketchbook/
---

# Open source contributions

## Polkadot SDK PRs
- [**polkadot-sdk PR #1445**](https://github.com/paritytech/polkadot-sdk/pull/1445) “removed `without_storage_info` from `pallet-collective`”, which lead to [**polkadot-sdk#1720**](https://github.com/paritytech/polkadot-sdk/pull/1720) “Associated type `Hasher` for `QueryPreimage`, `StorePreimage` and `Bounded`”. 
- [**polkadot-sdk PR #1747**](https://github.com/paritytech/polkadot-sdk/pull/1747) “Implement Inactive balance tracking in Assets pallet”. _Does it really need an article?_

## Tuxedo (and Substrate)
- Maybe I could write an article to say now that Joshy's working on Tuxedo, I am seeing with my own eyes that Substrate and FRAME are actually developed to be two separate entities, although this separation is not perfect. Of course some things can only come out if there's somebody working with only one of them, as it's the case with Tuxedo. I should mention the discussion in [**polkadot-sdk #211**](https://github.com/paritytech/polkadot-sdk/issues/211), my attempt to improve things in [**polkadot-sdk PR #2443**](https://github.com/paritytech/polkadot-sdk/pull/2443), and Joshy's PRs.
- I **must** write an article on how I managed to include transactions in the genesis block. Wait, now I'm thinking I could adapt this change to Substrate, instead of gatekeeping. Is it worth it? Is anybody ever going to use this feature outside of Tuxedo?

## Other open source projects
- [**paritytech/diener PR #45**](https://github.com/paritytech/diener/pull/45) “add support for `polkadot-sdk`”. I have used this tool while working on Tuxedo, even if its original intended use was for when Substrate, Polkadot and Cumulus were in separate repositories.
- I'm the maintainer of [**Off-Narrative-Labs/toml_sort**](https://github.com/Off-Narrative-Labs/toml_sort), a tool to sort TOML files. Well, I actually just wrote the GitHub Action and introduced it in various workflows. I will eventually tell Joshy we should publish it on GitHub Marketplace.
- I made [**0xPolygonZero/plonky2 PR #1335**](https://github.com/0xPolygonZero/plonky2/pull/1335) “restore `no-std` support” for plonky2, a Rust library for zk-SNARKs we might use in Tux0, in which I also added a CI test for target `wasm32-unknown-unknown`.
