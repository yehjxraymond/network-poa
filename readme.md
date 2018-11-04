# Simple POA network simulator with Parity

This project is used to run a local POA network using the Parity client. The main purpose is to conduct a series of benchmark test for POA networks. 

## Overview

The project spins up two nodes, `node0` and `node1`. `node0` will begin mining at a rate defined by the `stepDuration` parameter in `/config/chain.json`. `node1` will only start validating blocks from the 25th block as defined by `validators` parameter in `/config/chain.json`. 

## Running the network

```
docker-compose up
```

## Cleaning blockchain data

```
./prune.sh
```

## Todo

- Switch to docker volume to store `/chain` and `/data`
- Conduct benchmark test on the network