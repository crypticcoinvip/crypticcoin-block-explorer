# crypticcoin-block-explorer

Script to install and setup a CrypticCoin block explorer on Ubuntu 16.x or newer, or Debian 8+ for the CrypticCoin network.

## To run locally

On a fresh Ubuntu/Debian server, from a non-root user's home directory, run the following command:
```
wget -qO- https://raw.githubusercontent.com/crypticcoinvip/crypticcoin-block-explorer/master/install.sh | bash
```
or get and run 'install.sh' script manually.

To install only API:
```
wget -qO- https://raw.githubusercontent.com/crypticcoinvip/crypticcoin-block-explorer/master/install.sh | bash /dev/stdin --api-only
```

Then check config files and run ```bash crypticcoin-explorer/start_explorer.sh```.

The server runs in the foreground, and for production use scripts from "To setup production" section.

The block explorer will be available on http://localhost:3001/ and any additional IP addresses your server has bound to its network interface.
You can change the port in crypticcoin-explorer/bitcore-node.json.

All actions performed by the script are thouroughly commented.

## To setup production

##### Start in production mode:
```
bash crypticcoin-explorer/start_production_explorer.sh
```
##### Stop:
```
bash crypticcoin-explorer/stop_production_explorer.sh
```
##### Monitoring:
```
bash crypticcoin-explorer/monitor_production_explorer.sh
```



