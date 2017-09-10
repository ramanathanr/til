# To ssh and scp from Host OS to Cloudera QuickStart VM (on VirtualBox) 

1. In Guest OS, install openssh-server
> sudo yum install openssh-server

2. In VirtualBox menu, Machine -> Settings -> Network -> Adapter 1 -> Advanced, click on Port Forwarding button. 
Add a Port Forwarding rule with ssh (Name), 3022 (Host Port), 22 (Guest Port)

3. To ssh from Git Bash (Windows)
> $ ssh -p 3022 cloudera@127.0.0.1
password: cloudera

4. If you need to scp from Git Bash (Windows)
> $ scp -P 3022 <file> cloudera@127.0.0.1:/path


