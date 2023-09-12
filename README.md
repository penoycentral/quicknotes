# quicknotes

check password expiration
```
for user in $(cat /etc/passwd|cut -d: -f1); do echo $user; sudo chage --list $user |grep "Password expires"; done| paste -d " " - - | sed 's/Password
```

```
journalctl -b 0

```

```
chcon -t httpd_system_content_t /var/www/html/index.html
chcon --reference /var/www/html/ /var/www/html/index.html
```
