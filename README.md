# QuantisNet  
Forked from PIVX  

### How to update  
#### 1. Close current your local wallet  
  
#### 2. Download the latest local wallet from official github or file server  
https://github.com/QuantisDev/QuantisNet-Fork-New-Chain/releases  
http://45.76.62.99/files/  
Sorry, there isn't mac wallet at this point (1/31/2019)  
  
#### 3. Run the new wallet and confirm it's version  
Type "getinfo" on the debug console.  
You should see:  
"version" : 2000100,  
"protocolversion" : 72222,  
  
#### 4. Stop linux daemon and download new one (Only for people who are running own vps)  
You can use the script made by Llama.  
(Copy and paste one line at a time)  
wget https://raw.githubusercontent.com/LlamaOnDrugs/Quan/master/quan-mn-update.sh && chmod +x quan-mn-update.sh  
./quan-mn-update.sh  
  
Or you can update manually.  
./quantisnet-cli stop  
or  
/usr/local/bin/quantisnet-cli stop  
cd /usr/local/bin  
rm quantisnetd quantisnet-cli  
wget http://45.76.62.99/files/quantisnet-cli http://45.76.62.99/files/quantisnetd && chmod +x quantisnetd quantisnet-cli
./quantisnetd  
  
#### 5. Confirm daemon version  
./quantisnet-cli getinfo  
  
#### 6. start masternodes from local wallet  
You should see the protocol version will change to 72222 from 72221  
  
#### FAQ  
Q. When I start new local wallet an error windows appeard. What should I do?  
A. Backup quantisNET folder and delete folders and files except wallet.dat, masternode.conf, quantisnet.conf in quantisNET folder.  
   Then restart wallet.  

