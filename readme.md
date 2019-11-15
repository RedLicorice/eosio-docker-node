## EOSIO Node Docker Setup
**Sources**

EOSIO repository for binaries [EOS-Mainnet/eos](https://github.com/EOS-Mainnet/eos)

**Prerequisites**

Create the data directory, possibly populate it with data from [EOS Node Tools](https://eosnode.tools) (broken at the moment)

```$ mkdir nodeos-data```

**Running**

```$ docker-compose up -d --build```

Node will start syncing blocks data and expose on ports 8888 for RPC, 9876 for P2P