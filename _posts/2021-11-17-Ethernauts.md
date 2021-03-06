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

Now this was a quite confusing for me. I had to read quite a bit about the [fallback function](https://docs.soliditylang.org/en/v0.5.10/contracts.html#fallback-function) methods and what they are used for. So a fallback function is basically created so that the contract can receive ETH directly without calling any of the other functions. This must be a `payable` and have `external` visibility. A bad practice is including key logic elements within this function. This can give hackers a way into the smart contract. We can trigger a `fallback` function by 
 - Calling a function that doesn’t exist inside the contract, or
 - Calling a function without passing in required data, or
 - Sending Ether without any data to the contract

In this level, the fallback function is the last function. The idea I had was to just send the contract some ether and I would then be able to claim ownership as `owner = msg.sender` would be executed. Then I would run withdraw to pick up all that sweet ETH.
` contract.contribute({from: player, value:toWei("0.0001")})
	
  contract.sendTransaction({
    from: player,
    value: toWei("0.0009")
  })
  // Check if you are the owner
  await contract.owner();
 
  //Get out all the ETH
  contract.withdraw()
`


### LEvel 2

This was an easier one after going through the previous example and getting the syntax of all those console correct. I was able to gain ownership by just calling the old constructor `Fal1out`.

### Level 3


