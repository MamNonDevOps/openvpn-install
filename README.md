### Installation

```
sudo apt update -y
wget https://git.io/vpn -O openvpn-ubuntu-install.sh
chmod -v +x openvpn-ubuntu-install.sh
bash openvpn-ubuntu-install.sh
```

Public IPv4 address / hostname:

=> Enter `public ip of instances`


Which protocol should OpenVPN use?
   1) UDP (recommended)
   2) TCP

=> UDP is faster


What port should OpenVPN listen to?

=> default port 1194


Select a DNS server for the clients:
   1) Current system resolvers
   2) Google
   3) 1.1.1.1
   4) OpenDNS
   5) Quad9
   6) AdGuard

=> whatever! chọn gì cũng đc


Enter a name for the first client:

=> az-tech


The client configuration is available in: /root/az-tech.ovpn


### Download configuration file

Open TCP port 8000 on firewall or security groups


Run command
```
cd /root && python3 -m http.server
```


Open web browser, access url: `public ip of instances`:8000


Click to download file
