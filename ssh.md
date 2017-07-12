**Local Port Forwarding**
```
ssh -L <local_port>:destination.com:<destination_port> user@example.com
```

**Remote Port Forwarding**
```
ssh -R <remote_port>:localhost:<local_port> user@destination.com
```

To avoid opening a shell whenever we create a tunnel, use -nNT flags
