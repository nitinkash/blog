---
toc: false
layout: post
categories: ["Ethereum", "Smart Contracts"]
title: Towards becoming an Ethernaut
description: "Covers my experience hacking Smart Contracts on Ethereum"  
hide: false
---
So I got into the ttech involved in Crypto recently and builst some toy application on Ethereum and Solana. I wanted to gtake a step back and learn about hacking smart contracts before moving further. I found this game on [Open Zepplin](https://openzeppelin.com/) called [Ethernauts](https://ethernaut.openzeppelin.com/). Couldn't find a lot of info for a noob like me to follow, so I thought I'd write about how I progress down this. I am not giving all the directions and am just trying to give you a sense of where I got stuck and what I did to get out.

### Level 0

So this level was pretty straightforward. You just start off with `console.info()` and just follow the clues to get you to the password and then authenticate to the next level.

### Level 1

Now this was a quite confusing for me. I had to read quite a bit about the [fallback function](https://docs.soliditylang.org/en/v0.5.10/contracts.html#fallback-function) methods and what they are used for. So a fallback function is basically created so that the contract can receive ETH directly without calling any of the other functions. This must be a `payable` and have `external` visibility. In this level, the fallback function is the last function. The idea I had was to just send the contract some ether and I would then be able to claim ownership as `owner = msg.sender` would be executed. Then I would run withdraw to pick up all that sweet ETH.



