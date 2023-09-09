# quicknotes

check password expiration
```
for user in $(cat /etc/passwd|cut -d: -f1); do echo $user; sudo chage --list $user |grep "Password expires"; done| paste -d " " - - | sed 's/Password
```
