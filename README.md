# autovpn3
Autovpn3 script ready for pleasant using.

## Installation

1. `git clone https://github.com/Ryllaz/autovpn3.git`
2. `cd autovpn3`
3. `chmod +x autovpn3`
4. (optional) `sudo mv autovpn3 /usr/local/bin/autovpn3`. Then you will be able to run this script globally: `sudo autovpn3`.

## Usage

1. `cd /path/to/autovpn3`
2. `sudo ./autovpn3`

You can get help information by:  
`sudo ./autovpn3 --help`

## Config

You can override next ENV variables:

```bash
country='US' # empty for any or JP, KR, US, TH, etc.
useSavedVPNlist=0 # set to 1 if you don't want to download VPN list every time you restart this script, otherwise set to 0
useFirstServer=0 # set the value to 0 to choose a random VPN server, otherwise set to 1 (maybe the first one has higher score)
vpnList='/tmp/vpns.tmp'
proxy=0 # replace with 1 if you want to connect to VPN server through a proxy
proxyIP=''
proxyPort=8080
proxyType='socks' # socks or http
```

Also you can set any variable above as script parameter. Like:  
`sudo ./autovpn3 --country=US --proxyPort=8080`

