## Ping Sweep Subnet Linux
```bash
    for i in `seq 1 255`; do ping -c 1 192.168.1.$i | tr \\n ' ' | awk '/1 received/ {print $2}'; done
```

found [here](http://etherealmind.com/tech-notes-ping-sweep-ip-subnet/)
