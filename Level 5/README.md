
### Description
The password for the next level is stored in a file somewhere under the inhere directory and has all of the following properties:

- human-readable
- 1033 bytes in size
- not executable

### Solution
```bash
bandit5@bandit:~$ ls
inhere
```
```bash
bandit5@bandit:~$ find inhere/ -size 1033c
inhere/maybehere07/.file2
```
```bash
bandit5@bandit:~$ file inhere/maybehere07/.file2
inhere/maybehere07/.file2: ASCII text, with very long lines (1000)
```
```bash
bandit5@bandit:~$ ls -l inhere/maybehere07/.file2
-rw-r----- 1 root bandit5 1033 Apr 10 14:23 inhere/maybehere07/.file2
```
```bash
bandit5@bandit:~$ cat inhere/maybehere07/.file2
HWasnPhtq9AVKe0dmk45nxy20cvUa6EG
```
