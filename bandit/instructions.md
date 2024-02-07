# Bandit Notes

This is a unix instruction set to complete the OverTheWire Bandit challenge series. <br>
https://overthewire.org/wargames/bandit/

## Level 0 &rarr; Level 1

Password : bandit0

- ssh bandit0@bandit.labs.overthewire.org -p 2220

Highlights: use of ssh

## Level 1 &rarr; Level 2

- ls
- cat readme

Password : NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL

- exit
- ssh bandit1@bandit.labs.overthewire.org -p 2220

Highlights: use of ls and cat

## Level 2 &rarr; Level 3

- ls
- cat ./-

Password : rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi

- exit
- ssh bandit2@bandit.labs.overthewire.org -p 2220

Highlights: special uses of cat

## Level 3 &rarr; Level 4

- ls
- cat "spaces in this filename"

Password : aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG

- exit
- ssh bandit3@bandit.labs.overthewire.org -p 2220

Highlights: special uses of cat continued

## Level 4 &rarr; Level 5

- ls
- cd inhere
- ls -A
- cat .hidden

Password : 2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe

- exit
- ssh bandit4@bandit.labs.overthewire.org -p 2220

Highlights: hidden files

## Level 5 &rarr; Level 6

- ls
- cat inhere/*
- cd inhere
- ls
- cat ./-file07

Password : lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR

- exit
- ssh bandit5@bandit.labs.overthewire.org -p 2220

Highlights: multiple files and use of recursion

## Level 6 &rarr; Level 7

- ls
- man find
- find -size 1033c
- cat inhere/maybehere07/.file2

Password : P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU

- exit
- ssh bandit6@bandit.labs.overthewire.org -p 2220

Highlights: use of man and find

## Level 7 &rarr; Level 8

- ls -A
- find / -user bandit7 -group bandit6 -size 33c 2>/dev/null
- cat /var/lib/dpkg/info/bandit7.password

Password : z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S

- exit
- ssh bandit7@bandit.labs.overthewire.org -p 2220

Highlights: extended use of find

## Level 8 &rarr; Level 9

- ls
- man grep
- grep millionth data.txt

Password : TESKZC0XvTetK0S9xNwm25STk5iWrBvP

- exit
- ssh bandit8@bandit.labs.overthewire.org -p 2220

Highlights: use of grep

## Level 9 &rarr; Level 10

- ls
- man uniq
- sort data.txt | uniq -u

Password : EN632PlfYiZbn3PhVK3XOGSlNInNE00t

- exit
- ssh bandit9@bandit.labs.overthewire.org -p 2220

Highlights: use of uniq, sort, and piping

## Level 10 &rarr; Level 11

- ls
- man strings
- man grep
- strings data.txt | grep -a ===

Password : G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s

- exit
- ssh bandit10@bandit.labs.overthewire.org -p 2220

Highlights: use of strings and grep

## Level 10 &rarr; Level 11

- ls
- man base64
- base64 -d data.txt

Password : 6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM

- exit
- ssh bandit11@bandit.labs.overthewire.org -p 2220

Highlights: use of base64

## Level 11 &rarr; Level 12

- ls
- man tr
- cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'

Password : JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv

- exit
- ssh bandit12@bandit.labs.overthewire.org -p 2220

Highlights: use of tr

## Level 12 &rarr; Level 13

- ls
- mkdir /tmp/youngr2
- cp data.txt /tmp/youngr2
- cd /tmp/youngr
- ls
- man xxd
- xxd -r data.txt decompressed.txt
- file decompressed.txt
- man gzip
- gunzip decompressed.txt
- mv decompressed.txt decompressed.txt.gz
- gunzip decompressed.txt
- ls
- file decompressed.txt
- man bzip2
- bunzip2 decompressed.txt
- file decompressed.txt.out
- mv decompressed.txt.out decompressed.txt.gz
- gunzip decompressed.txt.gz
- ls
- file decompressed.txt
- man tar
- mv decompressed.txt decompressed.txt.tar
- tar -xf decompressed.txt
- ls
- file data5.bin
- mv data5.bin data5.bin.tar
- ls
- file data6.bin
- mv data6.bin data6.bin.txt
- bunzip2 data6.bin.txt
- ls
- file data6.bin.txt.out
- tar -xf data6.bin.txt.out
- file data8.bin
- mv data8.bin data8.bin.gz
- gunzip data8.bin.gz
- file data8.bin
- cat data8.bin

Password : wbWdlBxEir4CaE8LaPhauuOo6pwRmrDw

- exit
- ssh bandit13@bandit.labs.overthewire.org -p 2220

Highlights: Compression techniques

## Level 13 &rarr; Level 14

- ls
- man ssh
- ssh -i sshkey.private bandit14@localhost -p 2220
- cat /etc/bandit_pass/bandit14

Password : fGrHPx402xGC7U7rXKDaxiWFTOiF0ENq

Highlights: Use of ssh keys

## Level 14 &rarr; Level 15

- man nc
- nc localhost 30000
- fGrHPx402xGC7U7rXKDaxiWFTOiF0ENq

Password : jN2kgmIXJ6fShzhT2avhotn4Zcka6tnt

- exit
- ssh bandit15@bandit.labs.overthewire.org -p 2220

Highlights: Use of netcat

## Level 15 &rarr; Level 16

- man openssl
- openssl s_client -help
- cat /etc/bandit_pass/bandit15
- openssl s_client localhost:30001
- jN2kgmIXJ6fShzhT2avhotn4Zcka6tnt

Password : JQttfApK4SeyHwDlI9SXGR50qclOAil1

- exit
- ssh bandit16@bandit.labs.overthewire.org -p 2220

Highlights: use of openssl to connect to localhost

## Level 16 &rarr; Level 17

- man nmap
- nmap -p 31000-32000 -sV localhost
- cat /etc/bandit_pass/bandit16
- openssl s_client localhost:31790
- JQttfApK4SeyHwDlI9SXGR50qclOAil1

copy key

- mkdir /tmp/bandit16
- cd /tmp/bandit16
- cat > sshkey16.private

paste key

- chmod 600 sshkey16.private
- ssh -i sshkey16.private bandit17@localhost -p 2220

Highlights: Use of port scanning and some file permissions

## Level 17 &rarr; Level 18

- man diff
- ls
- diff passwords.new passwords.old

Password : hga5tuuCLF6fFzUpnagiMN8ssu9LFrdg

- exit
- exit
- ssh bandit18@bandit.labs.overthewire.org -p 2220

Highlights: Use of diff

## Level 18 &rarr; Level 19


