[Back](README.md)  
# Masternode FAQ  

I receive ```g++: internal compiler error: Killed (program cc1plus)``` when I run ```sudo make -f makefile.unix```  
> This error is caused because your VPS doesn't have enough memory to compile. Use the following guide to setup swap space on your VPS, and then try running the command again. https://www.digitalocean.com/community/tutorials/how-to-add-swap-space-on-ubuntu-16-04  

My masternode shows to be running but I haven't received a reward in a while, or I'm not getting as many rewards as I have in the past.  
> Rewards shouldn't be used as an indicator if the node is functioning. A random algorithm is used for determining rewards and some days will yield more rewards than others. If you haven't received any rewards since the setup of your node or it's been more than 48 hours since your last reward, you probably have a configuration issue.  

When using ```./Escrowd masternode status``` it returns ```"status" : 9``` and ```"notCapableReason" : "Could not find suitable coins!"```   
> It's normal to see this when the node is operational. Use ```./Escrowd masternode debug``` and if you get ```masternode started remotely``` as a response, everything is good.  

My masternode shows to be started, but the time Active shows 00:00:00.  
> It can take up to 30 minutes for the active time to update, but if it still isn't updating after 30 minutes, check the Escrow.conf file on your masternode. If the last line of the config is like this:  
> ```masternodeaddr=address:8018 masternode=1 masternodeprivkey=privatekey```,  
> you need to seperate each parameter on it's own line like so:  
> ```masternodeaddr=address:8018```  
> ```masternode=1```  
> ```masternodeprivkey=privatekey```  

I am setting up multiple masternodes, do I need to have a private key for each one?  
> Yes, when setting up multiple masternodes you will have to generate a private key for each node.  

I have multiple masternodes that I need to get verified for Escodex payouts, do I need to do the verification process for each masternode?  
> Yes, you will have to submit each masternode for verification using the receive address for each masternode.  

