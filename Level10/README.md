### Solution
```bash
bandit10@bandit:~$ ls
data.txt
```
```bash
bandit10@bandit:~$ cat data.txt 
VGhlIHBhc3N3b3JkIGlzIGR0UjE3M2ZaS2IwUlJzREZTR3NnMlJXbnBOVmozcVJyCg==
```
```bash
bandit10@bandit:~$ base64 -d  data.txt 
The password is dtR173fZKb0RRsDFSGsg2RWnpNVj3qRr
```

