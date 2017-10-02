# bootstrap
Capricoin Blockchain bootstrap

Capricoin-QT/capricoind supports a special import feature: If the file "bootstrap.dat" is found in the Capricoin directory (C:\users\username\AppData\Roaming\Capricoin\), it will validate and import all blockchain data found in that file.

----------------------
What is bootstrap.dat?

It is a flat, binary file containing Capricoin blockchain data, from the genesis block through a recent height.
All versions automatically validate and import the file "bootstrap.dat" in the data directory.

------------------------
Who wants bootstrap.dat?

Anyone bringing up a new node using the reference client.  This is one method of accelerating the initial blockchain download process, while helping the Capricoin P2P network by offloading data download traffic from public P2P nodes.

-----------------------
Why should I trust you?

You don't have to; This is raw blockchain data.  The client will verify this data during import.
Independent third parties may generate their own bootstrap.dat, up to a recent height, and verify that the sha256sum matches that posted below.  
