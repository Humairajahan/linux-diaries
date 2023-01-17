# Share local directory over HTTP server in a LAN 

|Version Info| [![Python](https://img.shields.io/badge/python-v3.9.0-green)](https://www.python.org/downloads/release/python-3913/)  [![Platform](https://img.shields.io/badge/Platforms-Ubuntu%2022.04.1%20LTS%2C%20win--64-orange)](https://releases.ubuntu.com/20.04/) |
|----|----|



Traverse to the directory that you want to serve from your command line. 
```
cd <your-directory>
```
Initiate python's simpleHTTPserver module on your desired port.
```
python -m  http.server <port>
```
Check out your local setup's ip address using the following command.
```
ifconfig
```
Now, expose your port to the LAN users.
```
sudo ufw allow <port>
```
Now other LAN users have read access to your directory. Go to the url <ip-address>:<port>. The other users can also download the directory or the individual files as well using the wget command.
```
wget <ip-address>:<port>/..
```

