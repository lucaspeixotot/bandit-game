# Bandit Game(CTF)
This is the solution of bandit game. You can see about this game in [OverTheWire site](http://overthewire.org/wargames/)

## Solution
The topic "Level X" will show the command needed to pass the X level. This solution starts from level 5 because the levels below are trivial.

Basically after run the command the password will be obvious.

### Level 5
Run this command and copy the password for the next level.

```bash
$ find . -size 1033c -not -executable
```
### Level 6

```bash
$ find / -size 33c -user bandit7 -group bandit8 -exec cat {} \;
```
### Level 7

```bash
$ echo $(grep -e millionth data.txt) | cut -d " " -f2
```
### Level 8

```bash
$ sort data.txt | uniq -u
```
### Level 9

```bash
$ strings -n 20 data.txt | grep = | cut -d " " -f2
```

### Level 10
```bash
$ base64 -d data.txt | cut -d " " -f4
```

### Level 11

```bash
$ cat data.txt | tr 'A-MN-Za-mn-z' 'N-ZA-Mn-za-m' | cut -d " " -f4
```

