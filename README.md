# Beacon node validator docker compose

> [Docker compose](https://github.com/docker/compose) file for for running Ethereum 2.0 [prysm](https://github.com/prysmaticlabs/prysm) beacon node and validator on the [Topaz](https://beacon.etherscan.io/) network.

## Getting started

```bash
export PASSWORD=mysecretpassword

# (1) generate keys
docker-compose run generate_validator_keys

# (2) view public key
docker-compose run view_public_key

# (3) run beacon chain and validator
docker-compose up validator
```

1. Generate keypair and copy the deposit data. Visit [https://prylabs.net/participate](https://prylabs.net/participate) to acquire 32 ETH and submit the raw transaction deposit data.

2. Retrieve your public key and visit [https://beacon.etherscan.io](https://beacon.etherscan.io) to view the deposit inclusion progress and attestions once the node starts validating.

3. Run the the beacon chain node, validator, and [eth2stats](https://github.com/Alethio/eth2stats-client) client. Wait for chain to sync and for deposit inclusion which could take 3-7hrs.

## License

[MIT](LICENSE)
