# OverTheWire-Bandit
## Level 0

Connected to bandit.labs.overthewire.org 

![image](https://github.com/sapphire-clouds/OverTheWire-Bandit/assets/148193056/97234e2a-c943-4808-b010-8175a35893a6)


## Level 0 → Level 1
![image](https://github.com/sapphire-clouds/OverTheWire-Bandit/assets/148193056/5f734bcf-d0ec-4d5b-b708-abf329e5a1e9)

**Commands used=**

1. cd= change the working directory

2. ls=- list directory contents

3. cat= read files and print the output

4. Ctl+C= Break

**Password acquired= NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL**

## Level 1 → Level 2
Login using bandit1 as username and the password acquired in last level 

![image](https://github.com/sapphire-clouds/OverTheWire-Bandit/assets/148193056/edfe8a1b-ff33-4b08-ae37-3cf535d711fb)

**Commands used=**
cat ./-
1. A single dot(.) represents the current working directory
2. Forward slash (/) Separates the components of a filename
3. The use of "./" before the hyphen character "-" in the **cat** command is meant to specify that we want to access and display the contents of a file named "-" located in the current directory. 

*The hyphen character "-" itself, when used as a filename, can sometimes cause confusion because it's often interpreted as a special . However, by prefixing it with "./", we make it clear to the shell that you are referring to a file with the literal name "-".* 

**Password acquired= rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi**

## Level 2 → Level 3
![image](https://github.com/sapphire-clouds/OverTheWire-Bandit/assets/148193056/90db6bd6-b3b4-4cc5-b8e3-f09b946b3c7f)

A space in a filename can cause errors when loading a file or when transferring files between computers.

1. Single quote  (' ') preserves all special characters within the string

**Password acquired= aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG**
## Level 3 → Level 4

![image](https://github.com/sapphire-clouds/OverTheWire-Bandit/assets/148193056/083bb9a6-4e65-4afa-9d1f-0a0690f616df)

When working with filenames, a leading dot is the prefix of a "hidden" file, a file that an ls will not normally show

**Password acquired= 2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe**

## Level 4 → Level 5
![image](https://github.com/sapphire-clouds/OverTheWire-Bandit/assets/148193056/1e780a5a-c7f8-4cd9-9f4a-e02c4a584fe5)

1. The asterisk (*) is a wildcard character in Unix-like systems that matches any sequence of characters. In the context of the used command (cat ./*) , * is used to match all files in the current directory.
