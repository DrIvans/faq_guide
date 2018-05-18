# Masternode FAQ  

I receive ```g++: internal compiler error: Killed (program cc1plus)``` when I run ```sudo make -f makefile.unix```  
> This error is caused because your VPS doesn't have enough memory to compile. Use the following guide to setup swap space on your VPS, and then try running the command again. https://www.digitalocean.com/community/tutorials/how-to-add-swap-space-on-ubuntu-16-04  

My masternode shows to be running but I haven't received a reward in a while, or I'm not getting as many rewards as I have in the past.  
> Rewards shouldn't be used as an indicator if the node is functioning. A random algorithm is used for determining rewards and some days will yield more rewards than others. If you haven't received any rewards since the setup of your node or it's been more than 48 hours since your last reward, you probably have a configuration issue.  

When using ```./Escrowd masternode status``` it returns ```"status" : 9``` and ```"notCapableReason" : "Could not find suitable coins!"```   
> It's normal to see this when the node is operational. Use ```./Escrowd masternode debug``` and if you get ```masternode started remotely``` as a response, everything is good.  
