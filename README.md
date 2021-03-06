## tBTC Network Subgraph

This subgraph indexes and exposes in GraphQL all the event data related to the tBTC Network contracts, providing an easy access to :

- Tracking TDTs
- Tracking minting
- New deposits per day
- Redemptions per day
- Total ETH bonded
- Mint transaction
- Deposit status
- tBtc holders
- ETH bonded

A live version of this subgraph can be found [here](https://thegraph.com/explorer/subgraph/suntzu93/tbtc), along with useful queries and examples already available on the playground.

### Example

Query token info: 

curl -X POST -H "Content-Type: application/json" --data '{"query":"{tbtctokens{id,name,address,totalMint,totalBurn,totalSupply,currentTokenHolders}}","variables":null}' https://api.thegraph.com/subgraphs/name/suntzu93/tbtc
