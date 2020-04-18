# TDC-Desktop-Wallet
Graphical wallet for TDC. For TDC project info see github.com/neiros/TDC

## Installation:

### On Ubuntu 16.04 LTS

- *Optional:* make sure you are up to date.
```
sudo apt update && sudo apt upgrade
```

- Install the dependencies:
```
sudo apt-get install build-essential git autoconf libtool libssl-dev libboost-all-dev libdb++-dev libgmp-dev qt4-qmake libqt4-dev
```

- Clone this repository:
```
git clone --recursive https://github.com/prism-lab/TDC-Desktop-Wallet.git
```

- Fix permissions:
```
cd TDC-Desktop-Wallet/tdc/src/leveldb && chmod +x build_detect_platform
```

- Return to project folder:
```
cd .. && cd .. && cd ..
```

- Build the source code:
```
qmake TDC-qt.pro USE_UPNP=-
make
```
