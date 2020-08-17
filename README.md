THECASH (TCH) integration/staging repository
======================================

THECASH is a cutting edge cryptocurrency, with many features not available in most other cryptocurrencies.
- 100% Proof of Stake 3.0 Consensus protocol, allowing very low transaction fees and energy expenditure, and staking rewards to all participants in the network.
- Masternode technology used to secure the network and provide additional features. Each Masternode is secured with collateral of 10000 TCH.
- Decentralized blockchain voting utilizing Masternode technology. The blockchain will distribute monthly treasury funds based on successful proposals submitted by the community and voted on by the Masternodes.


Quick installation of the THECASH daemon under linux.

Installation of libraries (using root user):

    add-apt-repository ppa:bitcoin/bitcoin -y
    apt-get update
    apt-get install -y build-essential libtool autotools-dev automake pkg-config libssl-dev libevent-dev bsdmainutils
    apt-get install -y libboost-system-dev libboost-filesystem-dev libboost-chrono-dev libboost-program-options-dev libboost-test-dev libboost-thread-dev
    apt-get install -y libdb4.8-dev libdb4.8++-dev

Cloning the repository and compiling (use any user with the sudo group):

    cd
    git clone https://github.com/thenode-foundation/THECASH.git
    cd THECASH
    ./autogen.sh
    ./configure
    sudo make install
    cd src
    sudo strip thecashd
    sudo strip thecash-cli
    sudo strip thecash-tx
    cd ..

Running the daemon:

    thecashd 

Stopping the daemon:

    thecash-cli stop

Demon status:

    thecash-cli getinfo
    thecash-cli mnsync status



## Coin Specs ##
<table>
<tr><td>Algo</td><td>Quark</td></tr>
<tr><td>Block Time</td><td>60 Seconds</td></tr>
<tr><td>Difficulty Retargeting</td><td>Every Block</td></tr>
<tr><td>Max Coin Supply</td><td>1000000000 TCH</td></tr>
<tr><td>Masternode Collateral</td><td>10000 TCH</td></tr>
<tr><td>Block Reward</td><td>695 TCH</td></tr>
</table>


More information at [THECASH](https://thecash.asia/)