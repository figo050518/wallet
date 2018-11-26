1 geth私有网络启动：
geth --networkid 15 --dev --dev.period 1 --rpc --rpcapi "db,eth,net,web3,miner,personal"   --rpccorsdomain "*" --rpcaddr "0.0.0.0" --rpcport "8545"   console 2>>log

2 miner.start()开始挖矿

3 转账：
    eth.sendTransaction({from: "0x4ff273e197f0fee97be31308e6bd9f444b5317f4", to: "0x80851fc08b7d741734766050a95d05a9220bafc3", value: web3.toWei(100, "ether")}) 