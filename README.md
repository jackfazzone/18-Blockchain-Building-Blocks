# ZBank Blockchain Guide

## Starting the Network
1. Open the bash terminal by pressing the windows key, typing bash, and hitting enter.

2. Enter "cd Blockchain-Tools" to enter the directory where the network will be started from.

3. Enter "./geth --datadir node1 init zbank_network.json" to initialize the first node and then enter "./geth --datadir node2 init zbank_network.json" to initialize the second node [see photo below].
    a. The "datadir" flag will specify to the geth tool the node-specific data directory to use to initialize each respective node.
    ![Node_Initialization](ZBank_network\Screenshots\Node_Intitalization.png)
4. Open a second bash terminal window.
5. In the first terminal window, enter "./geth --datadir node1 --unlock "F32D7f28f4B2B2E89BB256A1Dc7a1315feAF4DE9" --mine --rpc --allow-insecure-unlock," and then enter the password provided in the "Node_Info" text document to begin the first node mining [see photo below].
![Node1_Mining](ZBank_network\Screenshots\Node1_Mining.png)
6. In the second terminal window, repeat step 2, and then enter "./geth --datadir node2 --unlock "86c07990916463beCe9020bf89c80c1cdd6Ea9Ad" --mine --port 30304 --bootnodes "enode://1603ee474f0ce2aecb336cd0521a352c141ea0b1b303f85bacf92502c5172a9ad9402478708ff2e76e10e20eaea5eec7dc6ae9e8f7c4f6874868cc198dcb38b7@127.0.0.1:30303" --ipcdisable --allow-insecure-unlock," then enter the password provided in the "Node_Info" text document to begin the second node mining [see photo below].
![Node2_Mining](ZBank_network\Screenshots\Node2_Mining.png)

## Connecting to the Network through MyCrypto & Sending Transaction

1. Open the MyCrypto application.

2. Click "Change Network" on the left pane and then scroll down to "zbank_network" and click on it [see photo below].

![Change_Network](ZBank_network\Screenshots\Change_Network.png)

3. To send a transaction, click "View & Send" on the left pane, and then on "Keystore File" in the center of the bottom [photo below].

![MyCrypto](ZBank_network\Screenshots\MyCrypto.png)

4. When prompted, select the keystore file in the folder corresponding to the node from which you would like to send a transaction, enter the password provided in the "Node_Info" text document, and click "Unlock."

5. Enter the address for the other node, provided in the "Node_Info" text document, and the amount of Ether you would like to send.
![Send_Transaction](ZBank_network\Screenshots\Send_Transaction.png)

6. To view confirmation of your transaction, copy the transaction ID from the pop-up window, click "TX Status" from the left sidebar, paste the transaction ID, and click "Check TX Status" for details.
![Transaction_Confirmation](ZBank_network\Screenshots\Transaction_Confirmation.png)

## Network Information

Blocktime: 15 seconds

Chain ID: 123

