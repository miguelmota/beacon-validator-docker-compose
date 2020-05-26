# Beacon node validator docker compose

> [Docker compose](https://github.com/docker/compose) file for for running Ethereum 2.0 [prysm](https://github.com/prysmaticlabs/prysm) beacon node and validator on the [Topaz](https://beacon.etherscan.io/) network.

## Getting started

```bash
export PASSWORD=mysecretpassword

# generate keys
docker-compose run generate_validator_keys

# run beacon chain and validator
docker-compose up validator
```

## License

[MIT](LICENSE)
