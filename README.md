BFT
===
BFT serves an essential role in the bitfrog mechanism. It supports people to play games with bitcoins directly by serving as a bitcoin subchain. It integrates with bitcoin via a pegging process. You may find more in Leopard’s blog http://bitfrog.io/how-do-we-design-bitfrog/.

Website: http://bitfrog.io
BFT Specifications
===
- Ticker: BTC
- Block time: 30 seconds
- Pure Proof-of-Stake via integration to BFS

BFT Client
===
Source: To Be Released

```
Prerequisite :
1. Download and run BFS v0.8.6.3 with parameters -testnet and -gen

Window:
1.    Download all three components: 
	a)    BFS v0.8.6.3 (link)
	b)    bitfrogbtcd
	c)    BFT

2. Start BFS with -server and -testnet
3. Create a folder for BFT
4. Move bft-qt.exe and bitfrogbtcd into your BFT folder
5. Go to your C:\Users\You_User_Name\AppData\Roaming\BFT Directory and create a bft.conf file.
6. Go to your C:\Users\You_User_Name\AppData\Roaming\Bitfrogbtc Directory and create a bitcoin.conf file.
7. Start bitfrogbtcd.exe -testnet
8. Start bft-qt.exe

Mac and Linux:
To Be Released

```

Sample bft.conf file
===
```
gen=1
testnet=1
btcport=18332
btcrpcuser=btcrpcuser
btcrpcpassword=YourBTCSuperGreatPasswordNumber_DO_NOT_USE_THIS_OR_YOU_WILL_GET_ROBBED
bfsport=12321
bfsrpcuser=bfsrpcuser
bfsrpcpassword=YourBFSSuperGreatPasswordNumber_DO_NOT_USE_THIS_OR_YOU_WILL_GET_ROBBED

#You must set rpcuser and rpcpassword to secure the JSON-RPC api
rpcuser=rpcuser
rpcpassword=YourBFTSuperGreatPasswordNumber_DO_NOT_USE_THIS_OR_YOU_WILL_GET_ROBBED

```

Sample bitcoin.conf file
===
```
server=1
testnet=1

#You must set rpcuser and rpcpassword to secure the JSON-RPC api
rpcuser=btcrpcuser
rpcpassword=YourBTCSuperGreatPasswordNumber_DO_NOT_USE_THIS_OR_YOU_WILL_GET_ROBBED

```
