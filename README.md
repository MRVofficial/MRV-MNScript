# MRVCoin Masternode Setup Guide:


For **Ubuntu 16.04**
```
wget -q https://raw.githubusercontent.com/MRVofficial/MRV-MNScript/master/mrv_16.04.sh
sudo chmod +x mrv_16.04.sh
./mrv_16.04.sh
```
***

For **Ubuntu 18.04**
```
wget -q https://raw.githubusercontent.com/MRVofficial/MRV-MNScript/master/mrv_18.04.sh
sudo chmod +x mrv_18.04.sh
./mrv_18.04.sh
```
***

Do you want me to generate a masternode private key for you?[y/n]

- If you don't want to generate a masternode private key press **n**.

  > Next ask for Private key:
  
  > Enter your private key: Paste Your Masternode Private Key
  
  > Confirm your private key: Again Paste Your Masternode Private Key for confirmation

**OR**

- If you want to generate a masternode private key press  **y**.

 Enter VPS Public IP Address: Paste your VPS Address

 Wait till Node is fully Synced with blockchain.

`mrv_coin-cli getinfo`

When Node is Fully Synced enter the command below to check the masternode status.

`mrv_coin-cli getmasternodestatus`

You will get Masternode Successfully Started

# Create Masternode through Masternode Controller:

1. Go to MASTERNODES tab.
2. Click on Create Masternode Controller and go to NEXT.
3. Set Masternode Name (alias name) what you want to set.  (Ex. MRV_MN1) and go to NEXT.
4. Enter IP Address of VPS on which you want to start MN.
5. Click on NEXT So Your masternode Transaction done and wait for 15 Confirmation of it.
6. After 15 Confirmation you can Start MN from Console by fire Command. (EX. startmasternode alias false MRV_MN1)
7. After start from Cold wallet go to VPS and set all require data in mrv_coin.conf, restart daemon and start masternode by fire command
`mrv_coin-cli startmasternode local false`


