## wormholedb
### Install
* git clone https://github.com/SpendBCH/wormholedb.git
* cd wormholedb
* npm install
* npm install -g pm2
* pm2 install pm2-logrotate

### Configure
* Set your wormhole RPC host, RPC username, and RPC password in process.json
* Set the script location and cwd in process.json
* Set the block height to start syncing from in bitdb.json
  * The default sync from the first wormhole tx on mainnet

### Run
* pm2 start process.json

### Debug / Monitor
* pm2 logs wormholedb

Forked from: https://github.com/21centurymotorcompany/bitd