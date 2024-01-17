# week 1 lab report
## Examples of `cd`
1. using the command with no arguments:
```
  [user@sahara ~]$ cd
  [user@sahara ~]$
```
The working directory is home. `cd` change the current directory to be the argument. There is no argument for this command. Therefore, the current directory is not changing. 

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
  [user@sahara ~/lecture1]$
```
The working directory that the command was run is lecture1. `Hello.java` is not a directory, so it outputs an error message.

## Examples of `ls`
1. using the command with no arguments:
```
[user@sahara ~/lecture1]$ ls
Hello.class  Hello.java  messages  README
[user@sahara ~/lecture1]$
```
The working directory that the command was run is lecture1. `ls` will list all the files in the argument path. If there is no argument, `ls` will list the files in the current directory.

2.using the command with a path to a directory as an argument: 
```
[user@sahara ~/lecture1]$ ls messages
en-us.txt  es-mx.txt  fr.txt  zh-cn.txt
[user@sahara ~/lecture1]$ 
```
The working directory that the command was run is lecture1. `message` is the argument, so `ls messages` lists all the files inside `messages`.

3.using the command with a path to a file as an argument: 
```
[user@sahara ~/lecture1]$ ls Hello.java
Hello.java
[user@sahara ~/lecture1]$
```
The working directory that the command was run is lecture1. `Hello.java` is the argument. The path is `/home/lecture1/Hello.java`. There is a `Hello.java` in this path. Therefore, the output will be `Hello.java`.

## Examples of `cat`
1. using the command with no arguments:
  ```
  [user@sahara ~/lecture1]$ cat
  ```
The working directory that the command was run is lecture1. There is no output. `cat` command prints one or more files given by the paths. In this case, there is not input diretory. The command is waiting for a standard input.

2.using the command with a path to a directory as an argument: 
```
[user@sahara ~/lecture1]$ cat messages
cat: messages: Is a directory
[user@sahara ~/lecture1]$ 
```
The working directory that the command was run is lecture1. The argument `messages` is a diretory, not a files. Therefore, it outputs an error message saying tha `Is a directory`.

3.using the command with a path to a file as an argument: 
  ```
  [user@sahara ~/lecture1]$ cat Hello.java
  import java.io.IOException;
  import java.nio.charset.StandardCharsets;
  import java.nio.file.Files;
  import java.nio.file.Path;
  
  public class Hello {
    public static void main(String[] args) throws IOException {
      String content = Files.readString(Path.of(args[0]), StandardCharsets.UTF_8);    
      System.out.println(content);
    }
  }[user@sahara ~/lecture1]$ 
  ```
The working directory that the command was run is lecture1. `cat`command prints the code in the file `Hello.java`.
