# hddcoin-blockchain 

![Alt text](https://hddcoin.org/images/hdd_coin_logo_website_75.png)

HDDcoin is an eco-friendly decentralization blockchain based on the Proof of Space and Time (PoST) consensus pioneered by HDDcoin™. It maintains network robustness, in line with Satoshi Nakamoto's principles.

HDDcoin uses the powerful and secure Chialisp language for Smart Contracts, and supports digital money, global payments and applications. HDDcoin is not affiliated with HDDcoin Network, Inc., but uses their open-sourced software as its foundation.

Farming HDDcoin does not consume significant amounts of electricity, and utilizes hard drive space, instead of specialized computing hardware that most Proof of Work (PoW) consensus blockchains have come to demand. Moreover, since electrical energy costs for running hard drives is very minimal, due to this low cost of entry, HDDcoin will remain more decentralized and fair, and thus more secure than any Proof of Stake cryptocurrency.

HDDcoin core values include green cryptocurrency, long term value, building for the future, strength in community, and maintaining a huge team to ensure long term development.

The goal of HDDcoin is to reshape the global financial system through the power of the blockchain technology, powered by thousands of nodes maintained by the community, and with transparency and a commitment to the environment — thereby taking control from any central entity, person or organization, and giving that control back to the community.

**BLOCKCHAIN SPECIFICATION:**
- Launch date: July 8th 2021
- Cryptocurrency coin: HDD
- Lowest coin denomination: Bytes
- Conversion: 1 HDD = 1,000,000,000,000 Bytes
- Blocks per 24 hours target: 4,608
- Farmed rewards per block: 2 HDD
- Halving period for block rewards: 3 years

**BLOCKCHAIN RESOURCES:**
- Website: https://hddcoin.org/
- Explorer: https://alltheblocks.net/hddcoin
- Calculator: https://hddcoinforkscalculator.com/hddcoin
- HDDcoin DB: https://hddcoin.org/downloads/blockchain_v1_mainnet.sqlite

**COMMUNITIES AND SOCIAL CHANNELS:**
- Discord: https://discord.gg/AZdGSFnqAR
- Twitter: https://twitter.com/hddcoin
- YouTube: https://www.youtube.com/channel/UChJY3YEOTDBvFJ0vLFEc1Sw
- Facebook: https://www.facebook.com/HDDcoinNetwork
- Telegram: https://t.me/HDDcoin_Network
- Reddit: https://www.reddit.com/r/HDDcoinNetwork


***********************************************
# INSTALL INSTRUCTIONS:

You can install HDDcoin by building from source, or by using the latest binaries for your operating system.

(A.) To **install from available binaries**, download executables from the correct **Releases page**:

   - for solo farming, get them here ->
   https://github.com/HDDcoin-Network/hddcoin-blockchain/releases
   - for pool farming with FoxyPool (OG), get them here ->
   https://github.com/felixbrucker/hddcoin-blockchain/releases


(B.) To **build from source**, do the following:

```
# Update / Upgrade OS

   sudo apt-get update
   sudo apt-get upgrade -y

# Install Git

   sudo apt install git -y

# Checkout the correct source (either for solo or pool farming)

   ## for solo farming, use this source ## ->
   git clone https://github.com/HDDcoin-Network/hddcoin-blockchain.git

   ## for pool farming with FoxyPool (OG), use this source ## ->
   git clone https://github.com/felixbrucker/hddcoin-blockchain.git

  
# Install the Blockchain

   cd hddcoin-blockchain
   sh install.sh
   . ./activate
   hddcoin init

# Install and run the GUI

   sh install-gui.sh
   cd hddcoin-blockchain-gui
   npm run electron &
```

If the client does not find any connections automatically, you can add any of the following:

- introducer.hddcoin.org / Port: 28444
- dns-introducer.hddcoin.org / Port: 28444
- node-1.hddcoin.org / Port: 28444 / United States
- node-2.hddcoin.org / Port: 28444 / United States
- node-3.hddcoin.org / Port: 28444 / Hong Kong, China
- node-4.hddcoin.org / Port: 28444 / Munich, Germany
- node-5.hddcoin.org / Port: 28444 / Singapore, Singapore
- node-6.hddcoin.org / Port: 28444 / Bangalore, India
- node-7.hddcoin.org / Port: 28444 / Amsterdam, Netherlands
- node-8.hddcoin.org / Port: 28444 / United States
- node-9.hddcoin.org / Port: 28444 / United States
- node-10.hddcoin.org / Port: 28444 / United States
- node-11.hddcoin.org / Port: 28444 / United States
- node-12.hddcoin.org / Port: 28444 / United States
- node-13.hddcoin.org / Port: 28444 / United States
- node-14.hddcoin.org / Port: 28444 / United States

***********************************************
# UPDATE/UPGRADE INSTRUCTIONS:

You can update HDDcoin from a previous version by downloading and installing the latest executable for your operating system, available from the correct **Releases page**, as described above, or by building from source:

```
# Checkout the source and update

  cd hddcoin-blockchain
  . ./activate
  hddcoin stop -d all
  deactivate
  git fetch
  git checkout main
  git reset --hard FETCH_HEAD --recurse-submodules
  sh install.sh
  . ./activate
  hddcoin init

# Update the GUI

  cd hddcoin-blockchain-gui
  git fetch
  cd ..
  chmod +x ./install-gui.sh
  ./install-gui.sh
```
