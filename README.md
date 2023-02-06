# Chainlink Starknet Data Feeds

### Setting Up Starknet

- https://starknet.io/docs/quickstart.html
- `python3.9 -m venv ~/cairo_venv`
- `source ~/cairo_venv/bin/activate`
- `pip3 install ecdsa fastecdsa sympy`
- `brew install gmp`
- `pip3 install cairo-lang`

### Compiling and running first Cairo program

- `cairo-compile test.cairo --output test_compiled.json`
- `cairo-run --program=test_compiled.json --print_output --print_info --relocate_prints --tracer`
- open http://localhost:8100/

### Hardhat setup

- `npm install`

### Creating Starknet Account

- https://docs.starknet.io/documentation/getting_started/account_setup/
- `open ~/.starknet_accounts/starknet_open_zeppelin_accounts.json`

### Explorer

- https://testnet.starkscan.co/

### Chainlink Documentation Guide

- https://docs.chain.link/data-feeds/starknet

- `yarn build`
- `yarn deploy`
- `yarn readLatestRound`

- `yarn readLatestRoundOffChain`
- Or from CLI: `starknet call --address 0x2579940ca3c41e7119283ceb82cd851c906cbb1510908a913d434861fdcb245 --function latest_round_data --abi ./contracts/abis/aggregator_proxy_abi.json`

### Starknet Price Feeds

- https://docs.chain.link/data-feeds/price-feeds/addresses?network=starknet
