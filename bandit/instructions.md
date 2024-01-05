# Bandit Notes

This is a set of unix instructions to complete the OverTheWire Bandit challenge series. <br>
https://overthewire.org/wargames/bandit/

## Level 0 &rarr; Level 1

- ssh bandit0@bandit.labs.overthewire.org -p 2220
- bandit0

Highlights: use of ssh

## Level 1 &rarr; Level 2

- ls
- cat readme

Password : NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL

- exit
- ssh bandit1@bandit.labs.overthewire.org -p 2220
- NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL

Highlights: use of ls and cat

## Level 2 &rarr; Level 3

- ls
- cat ./-

Password : rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi

- exit
- ssh bandit2@bandit.labs.overthewire.org -p 2220
- rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi

Highlights: special uses of cat

## Level 3 &rarr; Level 4

- ls
- cat "spaces in this filename"

Password : aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG

- exit
- ssh bandit3@bandit.labs.overthewire.org -p 2220
- aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG

Highlights: special uses of cat continued

## Level 4 &rarr; Level 5

- ls
- cd inhere
- ls -A
- cat .hidden

Password : 2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe

- exit
- ssh bandit4@bandit.labs.overthewire.org -p 2220
- 2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe

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
- lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR

Highlights: multiple files and use of recursion

## Level 6 &rarr; Level 7

- ls
- man find
- find -size1033c
- cat inhere/maybehere07/.file2

Password : P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU

- exit
- ssh bandit6@bandit.labs.overthewire.org -p 2220
- P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU

Highlights: use of man and find

## Level 7 &rarr; Level 8

- ls -A
- find / -user bandit7 -group bandit6 -size 33c 2>/dev/null
- cat /var/lib/dpkg/info/bandit7.password

Password : z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S

- exit
- ssh bandit7@bandit.labs.overthewire.org -p 2220
- z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S

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