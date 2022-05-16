1 sudo -i
2 cd
2. ssh-keygen -t rsa ##in M1 , Press enter for each line
3. cat ~/.ssh/id_rsa.pub >> ~/.ssh/authorized_keys ##in M1
4. chmod og-wx ~/.ssh/authorized_keys ##in M1
5. tar -cvf ssh.tar .ssh/ ##in M1, This will create ssh.tar
6. ls ## U can see ssh.tar file now
mv ssh.tar /tmp/ move .ssh to temp
7. Now copy ssh.tar file in all other nodes with help of WinScp
Now Login in other nodes
8 sudo -i
9. move ssh.tar to root: mv /tmp/ssh.tar /root/
10 untar ssh.tar with command
Command- tar -xvf ssh.tar ##Run this command in all nodes
11. add all ip and hostnames in ti vi /etc/hosts of all servers.
