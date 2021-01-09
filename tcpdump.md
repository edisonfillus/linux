### Listen to all http traffic coming from a specific host (change host.example.com)
```shell
sudo tcpdump -A -s 0 'src host.example.com and tcp dst port 80 and (((ip[2:2] - ((ip[0]&0xf)<<2)) - ((tcp[12]&0xf0)>>2)) != 0)'
```

### Listen to all traffic in a specific port
```shell
sudo tcpdump -XX port 5155
```