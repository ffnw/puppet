## Debugging of Freifunk Supernode with multiple fastd instances

### Find the neigborths on the bat-testhood iface
```puppet
batctl -m bat-testhood o
```

### Test Speed
```puppet
wget --bind-address=10.18.8.1 http://speedtest.netcologne.de/test_1gb.bin
```

### Test Traceroute over the Ipv4 Exit
```puppet
traceroute -s 10.18.8.1 heise.de
```

### Debugging fastd Problems
```puppet
cat /var/log/syslog | grep "adding peer"
```

### Ping over any specific interfaces
```puppet
ping -I gre-ffrl-ber-a 8.8.8.8
```

