Task1: create and setup a new user account

```bash
sudo useradd anita -u 1171 -d /var/www/anita
```

In case the user was already created

```bash
sudo usermod -u 1171 -d /var/www/anita -m anita
```

check

```bash
id anita                # uid=1171(anita) gid=1002(anita) groups=1002(anita)
getent passwd 1171      # anita:x:1171:1002::/var/www/anita:/bin/bash
ls /var/www/anita
```
