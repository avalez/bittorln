Bitcoin node (pruned) in docker with tor and lightning

```
$ mkdir /Volumes/tor /Volumes/lnd /Volumes/bitcoin
$ sudo chown ... /Volumes/tor /Volumes/lnd /Volumes/bitcoin
$ cp torrc /Volumes/tor
$ cp lnd.conf /Volumes/lnd
$ cp bitcoin.conf /Volumes/bitcoin
$ RPCUSER=... RPCPASS=... docker compose up -d
$ docker exec -it bitcoin-node /usr/bin/bash      
root@5ced70fe97c5:/# bitcoin-cli -netinfo -rpcuser=... -rpcpassword=...
```

Expect 'onion in' NOT TO BE 0


