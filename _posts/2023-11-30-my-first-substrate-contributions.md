---
layout: post
title:  "My first contributions to Substrate"
date:   2023-11-30 20:15:57 +0100
tags: rust polkadot open-source
---

I wanted to make something quick for the first post on this blog.

Although not very interesting, I wanted to share the first contributions I made to Substrate in January 2023, while I was attending the second [Polkadot Blockchain Academy](https://polkadot.network/development/blockchain-academy/) in Buenos Aires.

[**substrate PR #13232**](https://github.com/paritytech/substrate/pull/13232) implemented a feature we needed to optimise the NFT Chain prototype.  
Before this PR, it was impossible to directly check in a `StorageDoubleMap` or `StorageNMap` if any item was present under a key with a certain prefix. The only way to check this was to iterate over all the items with that prefix, and ensure that the iterator was empty, a very inefficient operation.

In [**substrate PR #13245**](https://github.com/paritytech/substrate/pull/13245) I implemented `mutate_exists` and `try_mutate_exists` for `ValueQuery`, requested in [**substrate #13133**](https://github.com/paritytech/substrate/issues/13133).  
I was quite confident with the storage abstractions now, and I wanted to contribute more.  
I wonder if anybody ever used this feature.

I wanted to thank one more time Shawn Tabrizi and Kian Paimani for pushing me to start contributing to Substrate. Are they ever going to read this?
