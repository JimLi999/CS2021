# linux-1

```
cat flag
```

# linux-2

```
ls
ls -l
ls -al
```

# linux-3

```
cat hex.txt
xxd -r -p hex.txt
```

# linux-4

```
cat base64.text
base64 -d bast64.txt
```

# linux-5

```
find / -name secret
```

```
cat hiddenFilePath
```

# linux-6

```
ps aux
```

```
root          77  0.0  0.0  24360  1664 pts/0    S    Oct12   0:00 socat TCP-LISTEN:2111,reuseaddr,fork EXEC:/bin/flag
```

```
nc 127.0.0.1 2111
```

# linux-7

```
netstat -ano
```

```
tcp        0      0 0.0.0.0:80              0.0.0.0:*               LISTEN      off (0.00/0/0)
```

```
curl http://127.0.0.1/
```

# linux-8

```
mkdir /tmp/A100E110

cd /tmp/A100E110

wget http://120.114.62.217/ForYou.tar.gz

ls //list files

tar zxvf ForYou.tar.gz
```

```
file ForYou

ForYou: ASCII text, with CRLF line terminators

```

```
cat ForYou
```

# linux-9

```
wget http://120.114.62.217/TobeExe

ls //list files
```

```
file TobeExe

TobeExe: ELF 32-bit LSB executable, Intel 80386, version 1 (SYSV), dynamically linked,
interpreter /lib/ld-linux.so.2, for GNU/Linux 2.6.32, BuildID[sha1]=10558357d3700c05f1426a6d2a09b920bda2e464, not stripped
```

```
ls -al TobeExe

-rw-r--r-- 1 lab lab 7348 Nov 15  2017 TobeExe
```

```
chmod +x TobeExe


ls -al TobeExe
-rwxr-xr-x 1 lab lab 7348 Nov 15  2017 TobeExe
```

```
./TobeExe
```

# linux-10

```
wget http://120.114.62.217/reverse
```

```
ls //list files

```
```
file reverse
chmod +x reverse
./reverse
```
```
strings reverse | grep flag
```
```
strings reverse | grep CTF
```
