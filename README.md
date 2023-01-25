<img width="1200" alt="Labs" src="https://user-images.githubusercontent.com/99700157/213291931-5a822628-5b8a-4768-980d-65f324985d32.png">

<p>
 <h3 align="center">Chainstack is the leading suite of services connecting developers with Web3 infrastructure</h3>
</p>

<p align="center">
  <a target="_blank" href="https://chainstack.com/build-better-with-ethereum/"><img src="https://github.com/soos3d/blockchain-badges/blob/main/protocols_badges/Ethereum.svg" /></a>&nbsp;  
  <a target="_blank" href="https://chainstack.com/build-better-with-bnb-smart-chain/"><img src="https://github.com/soos3d/blockchain-badges/blob/main/protocols_badges/BNB.svg" /></a>&nbsp;
  <a target="_blank" href="https://chainstack.com/build-better-with-polygon/"><img src="https://github.com/soos3d/blockchain-badges/blob/main/protocols_badges/Polygon.svg" /></a>&nbsp;
  <a target="_blank" href="https://chainstack.com/build-better-with-avalanche/"><img src="https://github.com/soos3d/blockchain-badges/blob/main/protocols_badges/Avalanche.svg" /></a>&nbsp;
  <a target="_blank" href="https://chainstack.com/build-better-with-fantom/"><img src="https://github.com/soos3d/blockchain-badges/blob/main/protocols_badges/Fantom.svg" /></a>&nbsp;
</p>

<p align="center">
  • <a target="_blank" href="https://chainstack.com/">Homepage</a> •
  <a target="_blank" href="https://chainstack.com/protocols/">Supported protocols</a> •
  <a target="_blank" href="https://chainstack.com/blog/">Chainstack blog</a> •
  <a target="_blank" href="https://docs.chainstack.com/quickstart/">Chainstack docs</a> •
  <a target="_blank" href="https://docs.chainstack.com/quickstart/">Blockchain API reference</a> •
  <a target="_blank" href="https://console.chainstack.com/user/account/create">Start for free</a> •
</p>

# EVM propagation speed tester

This simple project is a pure front-end web application. It measures how fast a node can get a transaction in its `txpool` when sent from a different node. It is installation free and easy to use.

Read the full article on the Chainstack blog:
* [EVM speed tester: Measure how fast nodes respond to transactions](https://chainstack.com/evm-speed-tester/)

## Project details

This serverless web app requires two WebSocket endpoints, one wallet address, and a private key. After the program starts, the transaction is initiated on both endpoints one after another. It is a simple transaction. The address (identified using the private key) repeatedly sends the network’s base currency (e.g., ether) to itself. So the user can see how fast both nodes received the transaction.

## Quick start

Clone this repository:

```sh
git clone https://github.com/akegaviar/EVM_Speed-tester.git
```

Open `index.html` in a browser to see it in action:

1. Enter the private key and your address.
2. Enter the amount of the base network currency (e.g., ether) to transfer in each transaction. The default value is 0.1 ether, the minimum value is 1 Wei.
3. Enter the address of the WebSocket endpoints; it usually starts with `ws://` or `wss://`.
4. Click **start**;
5. Wait until both connections are established; the speed test starts after that.

You can also test it on JSFiddle:

* [EVM progagation speed test JSFiddle](https://jsfiddle.net/wuzhong/ecau2sLm/11/)

## Prerequisites

* A web browser.
* Two WebSocket endpoints.

Deploy a node with Chainstack:

1. [Sign up with Chainstack](https://console.chainstack.com/user/account/create).  
1. [Deploy a node](https://docs.chainstack.com/platform/join-a-public-network).  
1. [View node access and credentials](https://docs.chainstack.com/platform/view-node-access-and-credentials). 
