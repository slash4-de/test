# test

You should use sentinel for service discovery (hey sentinel, I need a redis connection, who is the master now?)

You can check if it runs by calling `docker ps`.

You can check if sentinels works by (on linux use 127.0.0.1 on mac use your docker host ip):

``` bash
  bash-3.2$ telnet 192.168.99.100 27001
  Trying 192.168.99.100...
  Connected to 192.168.99.100.
  Escape character is '^]'.

  SENTINEL get-master-addr-by-name mymaster
  192.168.99.100
  7001
  quit
```

