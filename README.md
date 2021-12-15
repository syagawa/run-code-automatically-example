# run code automaticalliy in Linux example


## install

```bash
$ cp ./example-hello-service.py ./hello-service.py
$ cp ./example-hello.service ./hello.service
```
Edit <username> in ./hello.service

```bash
$ cp ./hello-service.py ~/
$ chmod a+x ~/hello-service.py
$ cp ./hello-service ~/
$ sudo cp ~/hello-service /etc/systemd/system/
```


## usage

### start
`$ systemctl start hello.service`

### stop
`$ systemctl stop hello.service`

### check status
`$ systemctl status hello.service`

### show logs
`$ journalctl -u hello -e`

### start hello.service in boot
`$ systemctl enable hello.service`

### not start hello.service in boot
`$ systemctl disable hello.service`
