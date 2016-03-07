# Debugging of Freifunk Supernode with multiple fastd instances

### Find the neigborths on the bat-testhood iface
```puppet
batctl -m bat-testhood o
```

### Test Speed
```puppet
wget --bind-address=10.18.8.1 http://speedtest.netcologne.de/test_1gb.bin
```

### Test Traceroute over der Ipv4 Exit
```puppet
traceroute -s 10.18.8.1 heise.de
```
