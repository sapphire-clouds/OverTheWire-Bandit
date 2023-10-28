# OverTheWire-Bandit
## Level 0

Connected to bandit.labs.overthewire.org 

![image](https://github.com/sapphire-clouds/OverTheWire-Bandit/assets/148193056/024375b4-f48d-4252-979e-79dbe0bfdc0a)



## Level 0 → Level 1
![image](https://github.com/sapphire-clouds/OverTheWire-Bandit/assets/148193056/3398dba5-6bc1-479a-8c93-e8a954b3b023)

**Commands used=**

1. cd= change the working directory

2. ls=- list directory contents

3. cat= read files and print the output

4. Ctl+C= Break

**Password acquired= NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL**

## Level 1 → Level 2
Login using bandit1 as username and the password acquired in last level 

![image](https://github.com/sapphire-clouds/OverTheWire-Bandit/assets/148193056/9c37f4ad-c81b-49f9-bf97-0f8ea2cd661a)

**Commands used=**
cat ./-
1. A single dot(.) represents the current working directory
2. Forward slash (/) Separates the components of a filename
3. The use of "./" before the hyphen character "-" in the **cat** command is meant to specify that we want to access and display the contents of a file named "-" located in the current directory. 

*The hyphen character "-" itself, when used as a filename, can sometimes cause confusion because it's often interpreted as a special . However, by prefixing it with "./", we make it clear to the shell that you are referring to a file with the literal name "-".* 

**Password acquired= rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi**

## Level 2 → Level 3
![image](https://github.com/sapphire-clouds/OverTheWire-Bandit/assets/148193056/f47a4ba9-debb-497b-87ac-78fcfb142ab2)

A space in a filename can cause errors when loading a file or when transferring files between computers.

1. Single quote  (' ') preserves all special characters within the string

**Password acquired= aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG**
## Level 3 → Level 4

![image](https://github.com/sapphire-clouds/OverTheWire-Bandit/assets/148193056/5810e2a6-361b-46f6-ac04-422f5a795f57)

When working with filenames, a leading dot is the prefix of a "hidden" file, a file that an ls will not normally show

**Password acquired= 2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe**

## Level 4 → Level 5
![image](https://github.com/sapphire-clouds/OverTheWire-Bandit/assets/148193056/bb3e5df9-cea7-4564-ac13-ae65bde13a68)

1. The asterisk (*) is a wildcard character in Unix-like systems that matches any sequence of characters. In the context of the used command (cat ./*) , * is used to match all files in the current directory.

**Password acquired= lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR**

## Level 5 → Level 6
![image](https://github.com/sapphire-clouds/OverTheWire-Bandit/assets/148193056/96c37a24-4a99-40e4-a727-9a4f27ade3ef)

**Password acquired= P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU**
## Level 6 → Level 7

![image](https://github.com/sapphire-clouds/OverTheWire-Bandit/assets/148193056/ddbe01ef-e27a-4f4c-b4f3-65fe0ea520b5)
 1. 2>/dev/null = discards any error messages generated by the *find* command.

**Password acquired= z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S**

## Level 7 → Level 8

![image](https://github.com/sapphire-clouds/OverTheWire-Bandit/assets/148193056/f532d2f7-3fb5-47d4-a2fb-8f1465df091e)

1. awk '/millionth/ {print $2}': awk command searches for lines that contain the word "millionth" and then prints the second field (word) after it, which should be the password.
2. strings: This command extracts printable character sequences from the file.
3. grep "millionth": This command searches the output of strings for the word "millionth" and displays the line containing it, which should include the password.
   
**Password acquired= TESKZC0XvTetK0S9xNwm25STk5iWrBvP**
    
## Level 8 → Level 9
![image](https://github.com/sapphire-clouds/OverTheWire-Bandit/assets/148193056/5b33c2f2-d7fb-4fbe-a1c6-319e3af69255)

1. sort: This command sorts the lines in the file.
2. uniq -u: uniq when used with the -u option, displays only unique lines, meaning lines that occur only once
   
**Password acquired= EN632PlfYiZbn3PhVK3XOGSlNInNE00t**

## Level 9 → Level 10
![image](https://github.com/sapphire-clouds/OverTheWire-Bandit/assets/148193056/7e26d0c1-0b74-44b9-8100-ee78cd4c277a)

**Password acquired= G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s**

## Level 10 → Level 11

![image](https://github.com/sapphire-clouds/OverTheWire-Bandit/assets/148193056/f0a305fc-5739-4650-861e-92fc1f816eaa)

**Password acquired= 6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM**

## Level 11 → Level 12

![image](https://github.com/sapphire-clouds/OverTheWire-Bandit/assets/148193056/93b1db72-fd08-4dc4-91f4-9850d13aab62)

1. tr= short for "translate," is a basic Unix utility that is used to translate or delete characters in a text
    
**Password acquired= JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv**

## Level 12 → Level 13

1. Create a temporary directory in /tmp using *mkdir*
2. Copy the "data.txt" file to the temporary directory using *cp*
3. Change the working directory to the temporary directory using *cd*

<pre>bandit12@bandit:~$ mkdir /tmp/uwu
mkdir: cannot create directory ‘/tmp/uwu’: File exists
bandit12@bandit:~$ cp data.txt /tmp/uwu
bandit12@bandit:~$ cd /tmp/uwu
bandit12@bandit:/tmp/uwu$</pre>


4. *cat* to see the content of the file

<pre>bandit12@bandit:/tmp/uwu$ cat data.txt
00000000: 1f8b 0808 6855 1e65 0203 6461 7461 322e  ....hU.e..data2.
00000010: 6269 6e00 013d 02c2 fd42 5a68 3931 4159  bin..=...BZh91AY
00000020: 2653 5948 1b32 0200 0019 ffff faee cff7  &SYH.2..........
00000030: f6ff e4f7 bfbc ffff bff7 ffb9 39ff 7ffb  ............9...
00000040: bd31 eeff b9fb fbbb b9bf f77f b001 3b2c  .1............;,
00000050: d100 0d03 d200 6868 0d00 0069 a00d 0340  ......hh...i...@
00000060: 1a68 00d0 0d01 a1a0 0001 a680 0003 46d4  .h............F.
00000070: 6434 3234 611a 340d 07a4 c351 068f 5000  d424a.4....Q..P.
00000080: 069a 0680 0000 0006 8006 8da4 681a 6868  ............h.hh
00000090: 0d06 8d00 6834 3400 d07a 9a00 01a0 0341  ....h44..z.....A
000000a0: ea1e a190 da40 3d10 ca68 3468 6800 00c8  .....@=..h4hh...
000000b0: 1a1a 1b50 0683 d434 d069 a0d0 3100 d000  ...P...4.i..1...
000000c0: 001e a680 00d0 1a00 d0d0 6864 d0c4 d0d0  ..........hd....
000000d0: 000c 8641 7440 0108 032e 86b4 4cf0 22bb  ...At@......L.".
000000e0: 6682 2b7e b3e2 e98d aa74 dacc 0284 330d  f.+~.....t....3.
000000f0: bbb2 9494 d332 d933 642a 3538 d27e 09ce  .....2.3d*58.~..
00000100: 53da 185a 505e aada 6c75 59a2 b342 0572  S..ZP^..luY..B.r
00000110: 249a 4600 5021 25b0 1973 c18a 6881 1bef  $.F.P!%..s..h...
00000120: 3f9b 1429 5b1d 3d87 68b5 804f 1d28 42fa  ?..)[.=.h..O.(B.
00000130: 16c2 3241 98fb 8229 e274 5a63 fe92 3aca  ..2A...).tZc..:.
00000140: 70c3 a329 d21f 41e0 5a10 08cb 888f 30df  p..)..A.Z.....0.
00000150: f3da ce85 418b 0379 6a65 cfa2 eeb7 9f01  ....A..yje......
00000160: 782c da0e 288b e0c3 fe13 7af5 45ab 2b22  x,..(.....z.E.+"
00000170: a432 bf2f e32d b9e6 1465 2296 d805 a45e  .2./.-...e"....^
00000180: d1c1 eacb 7483 6aac ca0e cf24 8864 bd40  ....t.j....$.d.@
00000190: 118c 644a 1dc6 a127 375c b7a6 c124 bdae  ..dJ...'7\...$..
000001a0: 6d31 63a0 a223 3ea0 61d4 bdf0 450f 56fb  m1c..#>.a...E.V.
000001b0: a546 8d34 08a2 4f1d 43d3 9063 404d dd43  .F.4..O.C..c@M.C
000001c0: b4f2 e65d bcb7 5932 0f5e 6802 3892 a988  ...]..Y2.^h.8...
000001d0: 443d 8e89 7e09 4fb0 499d ee4e 4470 46c0  D=..~.O.I..NDpF.
000001e0: 2ba6 7c62 234a 7f76 151b aec0 23ee 4a97  +.|b#J.v....#.J.
000001f0: bc64 e34c de8a 5724 a1c3 9b89 cd96 1879  .d.L..W$.......y
00000200: d560 0cbb 5c26 09e4 efaf 5b94 402a 7780  .`..\&....[.@*w.
00000210: 4d87 30ce b8a3 946e 72c1 a643 1db7 a060  M.0....nr..C...`
00000220: 6524 629c 0c7e 8e7b e0f8 820c d5cb 60a0  e$b..~.{......`.
00000230: 003c a584 d4c1 61ef eb02 3f65 3a54 a3a2  .<....a...?e:T..
00000240: a565 c154 34c2 b162 d206 1ff8 bb92 29c2  .e.T4..b......).
00000250: 8482 40d9 9010 b3a9 e478 3d02 0000       ..@......x=...</pre>

5. Reverse hashdump using *xxd* and saving the result to a file ("new" here)
<pre>bandit12@bandit:/tmp/uwu$ xxd -r data.txt > new</pre>


7. Determining the file type using *file*
8. Alter the file type by renaming it to specific file format using *mv*
9. Decompressing/unzip-ing the files using *gunzip* and *bzip2* and *tar*
10. repeat

<pre>
bandit12@bandit:/tmp/uwu$ file new
new: gzip compressed data, was "data2.bin", last modified: Thu Oct  5 06:19:20 2023, max compression, from Unix, original size modulo 2^32 573
bandit12@bandit:/tmp/uwu$ mv new new.gz
bandit12@bandit:/tmp/uwu$ gunzip new.gz

bandit12@bandit:/tmp/uwu$ file new
new: bzip2 compressed data, block size = 900k
bandit12@bandit:/tmp/uwu$ mv new new.bz2
bandit12@bandit:/tmp/uwu$ bzip2 -d new.bz2

bandit12@bandit:/tmp/uwu$ file new
new: gzip compressed data, was "data4.bin", last modified: Thu Oct  5 06:19:20 2023, max compression, from Unix, original size modulo 2^32 20480
bandit12@bandit:/tmp/uwu$ mv new new.gz
bandit12@bandit:/tmp/uwu$ gunzip new.gz

bandit12@bandit:/tmp/uwu$ file new
new: POSIX tar archive (GNU)
bandit12@bandit:/tmp/uwu$ mv new new.tar
bandit12@bandit:/tmp/uwu$ tar -xvf new
tar: new: Cannot open: No such file or directory
tar: Error is not recoverable: exiting now
bandit12@bandit:/tmp/uwu$ tar -xvf new.tar
data5.bin
bandit12@bandit:/tmp/uwu$ cat data5.bin

bandit12@bandit:/tmp/uwu$ file data5.bin
data5.bin: POSIX tar archive (GNU)
bandit12@bandit:/tmp/uwu$ tar -xvf data5.bin
data6.bin

bandit12@bandit:/tmp/uwu$ file data6.bin
data6.bin: bzip2 compressed data, block size = 900k
bandit12@bandit:/tmp/uwu$ mv data6.bin data6.bz2
bandit12@bandit:/tmp/uwu$ bzip2 -d data6.bz2
bandit12@bandit:/tmp/uwu$ cat data6

bandit12@bandit:/tmp/uwu$ file data6
data6: POSIX tar archive (GNU)
bandit12@bandit:/tmp/uwu$ tar -xvf data6
data8.bin

bandit12@bandit:/tmp/uwu$ file data8.bin
data8.bin: gzip compressed data, was "data9.bin", last modified: Thu Oct  5 06:19:20 2023, max compression, from Unix, original size modulo 2^32 49
bandit12@bandit:/tmp/uwu$ mv data8.bin data8.gz
bandit12@bandit:/tmp/uwu$ gunzip data8.gz
bandit12@bandit:/tmp/uwu$ cat data8
The password is wbWdlBxEir4CaE8LaPhauuOo6pwRmrDw
</pre>

**Password acquired= wbWdlBxEir4CaE8LaPhauuOo6pwRmrDw**

## Level 13 → Level 14

<pre>
 bandit13@bandit:~$ ls -la
total 24
drwxr-xr-x  2 root     root     4096 Oct  5 06:19 .
drwxr-xr-x 70 root     root     4096 Oct  5 06:20 ..
-rw-r--r--  1 root     root      220 Jan  6  2022 .bash_logout
-rw-r--r--  1 root     root     3771 Jan  6  2022 .bashrc
-rw-r--r--  1 root     root      807 Jan  6  2022 .profile
-rw-r-----  1 bandit14 bandit13 1679 Oct  5 06:19 sshkey.private
bandit13@bandit:~$ ssh -i sshkey.private bandit14@localhost
The authenticity of host 'localhost (127.0.0.1)' can't be established.
ED25519 key fingerprint is SHA256:C2ihUBV7ihnV1wUXRb4RrEcLfXC5CXlhmAAM/urerLY.
This key is not known by any other names
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Could not create directory '/home/bandit13/.ssh' (Permission denied).
Failed to add the host to the list of known hosts (/home/bandit13/.ssh/known_hosts).

                      This is an OverTheWire game server. 
            More information on http://www.overthewire.org/wargames

!!! You are trying to log into this SSH server on port 22, which is not intended.

bandit14@localhost: Permission denied (publickey).
</pre>

didn't specify the specific port hence the error 

<pre>
bandit13@bandit:~$ ssh -i sshkey.private -p 2220 bandit14@localhost
The authenticity of host '[localhost]:2220 ([127.0.0.1]:2220)' can't be established.
ED25519 key fingerprint is SHA256:C2ihUBV7ihnV1wUXRb4RrEcLfXC5CXlhmAAM/urerLY.
This key is not known by any other names
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Could not create directory '/home/bandit13/.ssh' (Permission denied).
Failed to add the host to the list of known hosts (/home/bandit13/.ssh/known_hosts).

 
bandit14@bandit:~$ cat /etc/bandit_pass/bandit14
fGrHPx402xGC7U7rXKDaxiWFTOiF0ENq
</pre>

### Summary
<pre>
bandit13@bandit:~$ ssh -i sshkey.private -p 2220 bandit14@localhost

bandit14@bandit:~$ cat /etc/bandit_pass/bandit14
fGrHPx402xGC7U7rXKDaxiWFTOiF0ENq
</pre>

1. ssh= used to OpenSSH remote login client
2. -i= Selects a file from which the identity (private key) for public key authentication is read.
3. -p= Port to connect to on the remote host


**Password acquired= fGrHPx402xGC7U7rXKDaxiWFTOiF0ENq**

## Level 14 → Level 15

<pre>
bandit14@bandit:~$ echo fGrHPx402xGC7U7rXKDaxiWFTOiF0ENq | nc localhost 30000
Correct!
jN2kgmIXJ6fShzhT2avhotn4Zcka6tnt
</pre>

1. echo - display a line of text
2. nc (netcat)= reads and writes data across networks from the command line.

**Password acquired= jN2kgmIXJ6fShzhT2avhotn4Zcka6tnt**

## Level 15 → Level 16

<pre>
bandit15@bandit:~$ echo jN2kgmIXJ6fShzhT2avhotn4Zcka6tnt | openssl s_client -connect localhost:30001 -quiet
Can't use SSL_get_servername
depth=0 CN = localhost
verify error:num=18:self-signed certificate
verify return:1
depth=0 CN = localhost
verify error:num=10:certificate has expired
notAfter=Oct 28 09:39:22 2023 GMT
verify return:1
depth=0 CN = localhost
notAfter=Oct 28 09:39:22 2023 GMT
verify return:1
Correct!
JQttfApK4SeyHwDlI9SXGR50qclOAil1
</pre>

1. openssl s_client: This command is part of the OpenSSL toolkit and is used to connect to SSL/TLS-encrypted services. It's commonly used for establishing secure connections to remote servers.
2. -connect: This part of the command specifies the target server and port to connect to.
3. -quiet: The -quiet option is used to suppress unnecessary output from the openssl s_client command.

**Password acquired= JQttfApK4SeyHwDlI9SXGR50qclOAil1**

## Level 16 → Level 17
 1. Searching for ports that have a server listening on them

<pre>
bandit16@bandit:~$ nmap -p 31000-32000 localhost
Starting Nmap 7.80 ( https://nmap.org ) at 2023-10-28 16:55 UTC
Nmap scan report for localhost (127.0.0.1)
Host is up (0.00015s latency).
Not shown: 996 closed ports
PORT      STATE SERVICE
31046/tcp open  unknown
31518/tcp open  unknown
31691/tcp open  unknown
31790/tcp open  unknown
31960/tcp open  unknown

Nmap done: 1 IP address (1 host up) scanned in 0.23 seconds
</pre>

2. Checking for which speak SSL and which don’t

<pre>
bandit16@bandit:~$ openssl s_client -connect localhost:31046 -quiet
80DBF0F7FF7F0000:error:0A0000F4:SSL routines:ossl_statem_client_read_transition:unexpected message:../ssl/statem/statem_clnt.c:398:

 bandit16@bandit:~$ openssl s_client -connect localhost:31518 -quiet
Can't use SSL_get_servername
depth=0 CN = localhost
verify error:num=18:self-signed certificate
verify return:1
depth=0 CN = localhost
verify error:num=10:certificate has expired
notAfter=Oct 28 09:39:22 2023 GMT
verify return:1
depth=0 CN = localhost
notAfter=Oct 28 09:39:22 2023 GMT
verify return:1

 bandit16@bandit:~$ openssl s_client -connect localhost:31691 -quiet
80DBF0F7FF7F0000:error:0A0000F4:SSL routines:ossl_statem_client_read_transition:unexpected message:../ssl/statem/statem_clnt.c:398:
bandit16@bandit:~$ openssl s_client -connect localhost:31790 -quiet
Can't use SSL_get_servername
depth=0 CN = localhost
verify error:num=18:self-signed certificate
verify return:1
depth=0 CN = localhost
verify error:num=10:certificate has expired
notAfter=Oct 28 09:39:22 2023 GMT
verify return:1
depth=0 CN = localhost
notAfter=Oct 28 09:39:22 2023 GMT
verify return:1

bandit16@bandit:~$ openssl s_client -connect localhost:31960 -quiet
80DBF0F7FF7F0000:error:0A0000F4:SSL routines:ossl_statem_client_read_transition:unexpected message:../ssl/statem/statem_clnt.c:398:
</pre>

3. Ports 31518 and 31790 have SSL certificates. Checking to find the one that we need

<pre>
bandit16@bandit:~$ echo JQttfApK4SeyHwDlI9SXGR50qclOAil1 | openssl s_client -connect localhost:31518 -quiet
Can't use SSL_get_servername
depth=0 CN = localhost
verify error:num=18:self-signed certificate
verify return:1
depth=0 CN = localhost
verify error:num=10:certificate has expired
notAfter=Oct 28 09:39:22 2023 GMT
verify return:1
depth=0 CN = localhost
notAfter=Oct 28 09:39:22 2023 GMT
verify return:1
JQttfApK4SeyHwDlI9SXGR50qclOAil1
</pre>

<pre>
 bandit16@bandit:~$ echo JQttfApK4SeyHwDlI9SXGR50qclOAil1 | openssl s_client -connect localhost:31790 -quiet
Can't use SSL_get_servername
depth=0 CN = localhost
verify error:num=18:self-signed certificate
verify return:1
depth=0 CN = localhost
verify error:num=10:certificate has expired
notAfter=Oct 28 09:39:22 2023 GMT
verify return:1
depth=0 CN = localhost
notAfter=Oct 28 09:39:22 2023 GMT
verify return:1
Correct!
-----BEGIN RSA PRIVATE KEY-----
MIIEogIBAAKCAQEAvmOkuifmMg6HL2YPIOjon6iWfbp7c3jx34YkYWqUH57SUdyJ
imZzeyGC0gtZPGujUSxiJSWI/oTqexh+cAMTSMlOJf7+BrJObArnxd9Y7YT2bRPQ
Ja6Lzb558YW3FZl87ORiO+rW4LCDCNd2lUvLE/GL2GWyuKN0K5iCd5TbtJzEkQTu
DSt2mcNn4rhAL+JFr56o4T6z8WWAW18BR6yGrMq7Q/kALHYW3OekePQAzL0VUYbW
JGTi65CxbCnzc/w4+mqQyvmzpWtMAzJTzAzQxNbkR2MBGySxDLrjg0LWN6sK7wNX
x0YVztz/zbIkPjfkU1jHS+9EbVNj+D1XFOJuaQIDAQABAoIBABagpxpM1aoLWfvD
KHcj10nqcoBc4oE11aFYQwik7xfW+24pRNuDE6SFthOar69jp5RlLwD1NhPx3iBl
J9nOM8OJ0VToum43UOS8YxF8WwhXriYGnc1sskbwpXOUDc9uX4+UESzH22P29ovd
d8WErY0gPxun8pbJLmxkAtWNhpMvfe0050vk9TL5wqbu9AlbssgTcCXkMQnPw9nC
YNN6DDP2lbcBrvgT9YCNL6C+ZKufD52yOQ9qOkwFTEQpjtF4uNtJom+asvlpmS8A
vLY9r60wYSvmZhNqBUrj7lyCtXMIu1kkd4w7F77k+DjHoAXyxcUp1DGL51sOmama
+TOWWgECgYEA8JtPxP0GRJ+IQkX262jM3dEIkza8ky5moIwUqYdsx0NxHgRRhORT
8c8hAuRBb2G82so8vUHk/fur85OEfc9TncnCY2crpoqsghifKLxrLgtT+qDpfZnx
SatLdt8GfQ85yA7hnWWJ2MxF3NaeSDm75Lsm+tBbAiyc9P2jGRNtMSkCgYEAypHd
HCctNi/FwjulhttFx/rHYKhLidZDFYeiE/v45bN4yFm8x7R/b0iE7KaszX+Exdvt
SghaTdcG0Knyw1bpJVyusavPzpaJMjdJ6tcFhVAbAjm7enCIvGCSx+X3l5SiWg0A
R57hJglezIiVjv3aGwHwvlZvtszK6zV6oXFAu0ECgYAbjo46T4hyP5tJi93V5HDi
Ttiek7xRVxUl+iU7rWkGAXFpMLFteQEsRr7PJ/lemmEY5eTDAFMLy9FL2m9oQWCg
R8VdwSk8r9FGLS+9aKcV5PI/WEKlwgXinB3OhYimtiG2Cg5JCqIZFHxD6MjEGOiu
L8ktHMPvodBwNsSBULpG0QKBgBAplTfC1HOnWiMGOU3KPwYWt0O6CdTkmJOmL8Ni
blh9elyZ9FsGxsgtRBXRsqXuz7wtsQAgLHxbdLq/ZJQ7YfzOKU4ZxEnabvXnvWkU
YOdjHdSOoKvDQNWu6ucyLRAWFuISeXw9a/9p7ftpxm0TSgyvmfLF2MIAEwyzRqaM
77pBAoGAMmjmIJdjp+Ez8duyn3ieo36yrttF5NSsJLAbxFpdlc1gvtGCWW+9Cq0b
dxviW8+TFVEBl1O4f7HVm6EpTscdDxU+bCXWkfjuRb7Dy9GOtt9JPsX8MBTakzh3
vBgsyi/sN3RqRBcGU40fOoZyfAMT8s1m/uYv52O6IgeuZ/ujbjY=
-----END RSA PRIVATE KEY-----

bandit16@bandit:~$ 
</pre>

Port 31790 is the one that we needed

4.ff

<pre>
bandit16@bandit:~$ echo "-----BEGIN RSA PRIVATE KEY-----
MIIEogIBAAKCAQEAvmOkuifmMg6HL2YPIOjon6iWfbp7c3jx34YkYWqUH57SUdyJ
imZzeyGC0gtZPGujUSxiJSWI/oTqexh+cAMTSMlOJf7+BrJObArnxd9Y7YT2bRPQ
Ja6Lzb558YW3FZl87ORiO+rW4LCDCNd2lUvLE/GL2GWyuKN0K5iCd5TbtJzEkQTu
DSt2mcNn4rhAL+JFr56o4T6z8WWAW18BR6yGrMq7Q/kALHYW3OekePQAzL0VUYbW
JGTi65CxbCnzc/w4+mqQyvmzpWtMAzJTzAzQxNbkR2MBGySxDLrjg0LWN6sK7wNX
x0YVztz/zbIkPjfkU1jHS+9EbVNj+D1XFOJuaQIDAQABAoIBABagpxpM1aoLWfvD
KHcj10nqcoBc4oE11aFYQwik7xfW+24pRNuDE6SFthOar69jp5RlLwD1NhPx3iBl
J9nOM8OJ0VToum43UOS8YxF8WwhXriYGnc1sskbwpXOUDc9uX4+UESzH22P29ovd
d8WErY0gPxun8pbJLmxkAtWNhpMvfe0050vk9TL5wqbu9AlbssgTcCXkMQnPw9nC
YNN6DDP2lbcBrvgT9YCNL6C+ZKufD52yOQ9qOkwFTEQpjtF4uNtJom+asvlpmS8A
vLY9r60wYSvmZhNqBUrj7lyCtXMIu1kkd4w7F77k+DjHoAXyxcUp1DGL51sOmama
+TOWWgECgYEA8JtPxP0GRJ+IQkX262jM3dEIkza8ky5moIwUqYdsx0NxHgRRhORT
8c8hAuRBb2G82so8vUHk/fur85OEfc9TncnCY2crpoqsghifKLxrLgtT+qDpfZnx
SatLdt8GfQ85yA7hnWWJ2MxF3NaeSDm75Lsm+tBbAiyc9P2jGRNtMSkCgYEAypHd
HCctNi/FwjulhttFx/rHYKhLidZDFYeiE/v45bN4yFm8x7R/b0iE7KaszX+Exdvt
SghaTdcG0Knyw1bpJVyusavPzpaJMjdJ6tcFhVAbAjm7enCIvGCSx+X3l5SiWg0A
R57hJglezIiVjv3aGwHwvlZvtszK6zV6oXFAu0ECgYAbjo46T4hyP5tJi93V5HDi
Ttiek7xRVxUl+iU7rWkGAXFpMLFteQEsRr7PJ/lemmEY5eTDAFMLy9FL2m9oQWCg
R8VdwSk8r9FGLS+9aKcV5PI/WEKlwgXinB3OhYimtiG2Cg5JCqIZFHxD6MjEGOiu
L8ktHMPvodBwNsSBULpG0QKBgBAplTfC1HOnWiMGOU3KPwYWt0O6CdTkmJOmL8Ni
blh9elyZ9FsGxsgtRBXRsqXuz7wtsQAgLHxbdLq/ZJQ7YfzOKU4ZxEnabvXnvWkU
YOdjHdSOoKvDQNWu6ucyLRAWFuISeXw9a/9p7ftpxm0TSgyvmfLF2MIAEwyzRqaM
77pBAoGAMmjmIJdjp+Ez8duyn3ieo36yrttF5NSsJLAbxFpdlc1gvtGCWW+9Cq0b
dxviW8+TFVEBl1O4f7HVm6EpTscdDxU+bCXWkfjuRb7Dy9GOtt9JPsX8MBTakzh3
vBgsyi/sN3RqRBcGU40fOoZyfAMT8s1m/uYv52O6IgeuZ/ujbjY=
-----END RSA PRIVATE KEY-----" | ssh -i - bandit17@bandit.labs.overthewire.org -p 2220
</pre>

## Level 17 → Level 18

<pre>
 bandit17@bandit:~$ diff passwords.old passwords.new
42c42
< p6ggwdNHncnmCNxuAt0KtKVq185ZU7AW
---
> hga5tuuCLF6fFzUpnagiMN8ssu9LFrdg
bandit17@bandit:~$ 
</pre>

1. The diff command will compare 2 files line by line and show you the differences

**Password acquired= hga5tuuCLF6fFzUpnagiMN8ssu9LFrdg**

## Level 18 → Level 19

![image](https://github.com/sapphire-clouds/OverTheWire-Bandit/assets/148193056/82219949-3a88-40c3-8447-957c2449e866)

**Password acquired= awhqfNnAbc1naukrpqDYcF95h7HoMTrC**

## Level 19 → Level 20

## Level 20 → Level 21
