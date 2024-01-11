# week 1 lab report
## Examples of `cd`
1. using the command with no arguments:
```
  [user@sahara ~]$ cd
  [user@sahara ~]$
```
The working directory is home. 'cd change the current directory to be the argument. There is no argument for this command. Therefore, the current directory is not changing. 

2. using the command with a path to a directory as an argument: 
```
  [user@sahara ~]$ cd lecture1
  [user@sahara ~/lecture1]$
```
  The working directory that the command was run is home. After the command run, the current directory set to be lecture1.

3. using the command with a path to a file as an argument: 
```
  [user@sahara ~/lecture1]$ cd Hello.java
  bash: cd: Hello.java: Not a directory
```
The working directory that the command was run is lecture1. `Hello.java` is not a directory, so the output is an error.

## Examples of `ls`
1. using the command with no arguments:
```
[user@sahara ~/lecture1]$ ls
Hello.class  Hello.java  messages  README
```
The working directory that the command was run is lecture1. `ls` will list all the files in the argument path. If there is no argument, `ls` will list the files in the current directory.

2.using the command with a path to a directory as an argument: 

3.using the command with a path to a file as an argument: 
