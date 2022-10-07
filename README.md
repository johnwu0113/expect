# Indirect SCP

## Information

[ssh-client]#  cat /etc/redhat-release

CentOS Linux release 7.9.2009 (Core)

[ssh-client]#  expect -v

expect version 5.45

---

## Delpoy 
1. Copy the index.php into the web directory.

---
## Desciption
[ssh-client] expect scp_file.exp [ssh-server] [username] [password] [indirect-server] 
spawn ssh [username]@[ssh-server] 

[username]@[ssh-server]'s password:[password]

[ssh-server]# /file scp [ssh-server's file] [indirect-server's username]@[indirect-server]:[folder] 
[indirect-server's username]@[indirect-server]'s password:[indirect-server's password]
[file]                                    100%   xxKB  xxKB/s   00:00
[ssh-server]# logout
