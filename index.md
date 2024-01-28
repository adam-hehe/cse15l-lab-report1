# Lab Report 1

## `cd` Command

```
  Input: [user@sahara ~]$ cd
  Output: [user@sahara ~]$
```
The working directory was `/home` when the command was ran. Having no arguments takes the user to the home directory. No error.

```
  Input: [user@sahara ~]$ cd lecture1
  Output: [user@sahara ~/lecture1]$ 
```
The working directory was `/home` when the command was ran. After the command was ran the directory was changed to `/home/lecture1`. Running the `cd`
command changes the directory to the given arguments if it can be found. No error.

```
  Input: [user@sahara ~/lecture1/messages]$ cd fr.txt
  Output: bash: cd: fr.txt: Not a directory
```
The working directory was `/lecture1/messages` when the command was ran and remained the same after. 
The command produced an error because `fr.txt` is a file and not a directory

```
  Input: [user@sahara ~/lecture1]$ ls
  Output: Hello.class  Hello.java  messages  README
```
The working directory was `/home/lecture1`. When `ls` is ran it lists all the files and directories that are contained within the working directory.
No error.

```
  Input: [user@sahara ~]$ ls lecture1
  Output: Hello.class  Hello.java  messages  README
```
The working directory was `/home`. When `ls` is ran with an directory it lists the files and directories that are contained within that given
directory. No error.

```
  Input: [user@sahara ~/lecture1/messages]$ ls fr.txt
  Output: Hello.class  Hello.java  messages  README
```
The working directory was `/lecture1/messages`. When `ls` is ran with an file it produces an error because the command only workds
with directories. Error because fr.txt is not a directory.

```
  Input: [user@sahara ~]$ cat
  Output:
```
The working directory was `/home`. When `cat` has no arguments it produces no output because there is nothing to print out to the terminal. This give no error but you have to exit the 
command.

```
  Input: [user@sahara ~]$ cat lecture1
  Output: cat: lecture1: Is a directory
```
The working directory was `/home`. When `cat` is given a directory as an argument it produces an error because it can only concatanate the contents of two files.

```
  Input: [user@sahara ~/lecture1/messages]$ cat fr.txt es-mx.txt
  Output: Bonjour le monde!
          ¡Hola Mundo!
```
The working directory was `/home/lecture1/messages`. When `cat` is given a file as an argument it will print out the contents of that file. If the `cat` command is given two arguments
it will combine the two and print them both out. No error.
