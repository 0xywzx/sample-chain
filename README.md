# sample-chain

```
account : 2780e0b7959b985864f8d787389224a2039a3b60
password : sample
```

```
$ git clone git@github.com:Yosuke-Aramaki/sample-chain.git
$ cd sample-chain
$ $ geth --datadir node1/ --syncmode 'full' --port 30311 --rpc --rpcaddr '0.0.0.0' --rpcport 8545 --rpccorsdomain "*" --rpcvhosts "*" --rpcapi 'personal,db,eth,net,web3,txpool,miner' --ws --wsapi 'eth,web3,net' --wsorigins='*' --wsaddr='0.0.0.0' --wsport 8546 --networkid 1515 --gasprice '0'
```

```
$ cd sample-chain
$ geth attach ipc:node1/geth.ipc
$ personal.unlockAccount(eth.coinbase,"sample",0)
$ mimer.start()
```
