# Send a message to another device connected over the same LAN

## Get started

Firstly, install `zenity` for displaying graphical dialog boxes.
```bash
sudo apt-get update
sudo apt-get install zenity
```
Copy the file `daemon.sh`. This applies for all the PCs you want to bind together along with your server PC.
```bash
chmod +x daemon.sh
bash daemon.sh
```
Now run the file `connect.sh` in your server PC.
```bash
bash connect.sh
```
If this opens a *subshell* terminal, that means the connection between the PCs has been set. If that is not the case, then ensure that `daemon.sh` is running in the client PCs as well. 

Now, in the subshell terminal, type in your intended message, sit back and Relax! 

Happy communicating!
