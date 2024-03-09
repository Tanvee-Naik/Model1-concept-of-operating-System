PART A

tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ cd ..
tanvee@LAPTOP-2EIP57DT:~/ShellProgram$ echo "Hello, World!"
Hello, World!
tanvee@LAPTOP-2EIP57DT:~/ShellProgram$ name="Productive"
tanvee@LAPTOP-2EIP57DT:~/ShellProgram$ touch file.txt
tanvee@LAPTOP-2EIP57DT:~/ShellProgram$ ls -a
.   Assignment2  Que2.sh  T2.sh  T4.sh  T6.sh  T8.sh
..  Que1.sh      T1.sh    T3.sh  T5.sh  T7.sh  file.txt
tanvee@LAPTOP-2EIP57DT:~/ShellProgram$ mv file.txt /path/to/directory/
mv: cannot move 'file.txt' to '/path/to/directory/': No such file or directory
tanvee@LAPTOP-2EIP57DT:~/ShellProgram$ mv file.txt Assignment2
tanvee@LAPTOP-2EIP57DT:~/ShellProgram$ chmod 755 script.sh
chmod: cannot access 'script.sh': No such file or directory
tanvee@LAPTOP-2EIP57DT:~/ShellProgram$ cd Assignment2
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ vi script.sh
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ chmod 755 script.sh
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ ./script.sh
ASSIGNMENT 2 PART A
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ ls -al
total 16
drwxr-xr-x 2 tanvee tanvee 4096 Mar  9 09:52 .
drwxr-xr-x 3 tanvee tanvee 4096 Mar  9 09:50 ..
-rw-r--r-- 1 tanvee tanvee   12 Mar  9 09:47 Part1.sh
-rw-r--r-- 1 tanvee tanvee    0 Mar  9 09:48 file.txt
-rwxr-xr-x 1 tanvee tanvee   40 Mar  9 09:52 script.sh
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ cat > file1.txt
pattern programming
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ grep "pattern" file.txt
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ cat file.txt |grep "pattern"
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ grep -i "pattern" file.tx
t
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ grep "pattern" file1.txt
pattern programming
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ kill PID
-bash: kill: PID: arguments must be process or job IDs
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ man  kill PID
No manual entry for PID
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ mkdir mydir && cd mydir && touch file.txt && echo "Hello, World!" > file.txt && cat file.txt
Hello, World!
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2/mydir$ ls -l | grep ".txt"
-rw-r--r-- 1 tanvee tanvee 14 Mar  9 10:01 file.txt
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2/mydir$ cat file1.txt file2.txt | sort | uniq
cat: file1.txt: No such file or directory
cat: file2.txt: No such file or directory
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2/mydir$ touch file2.txt
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2/mydir$ cp file2.txt
cp: missing destination file operand after 'file2.txt'
Try 'cp --help' for more information.
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2/mydir$ cp file1.txt file2.
txt
cp: cannot stat 'file1.txt': No such file or directory
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2/mydir$ cd ..
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ cd mydir
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2/mydir$ rm file2.txt
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2/mydir$ cd ..
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$  touch file2.txt
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ cp file1.txt file2.
txt
Command 'txt' not found, did you mean:
  command 'xt' from snap xt (0+git.99c6ce0)
  command 'tx' from deb transifex-client (0.14.2-1)
  command 'tst' from deb pvm-examples (3.4.6-3.2)
  command 'tgt' from deb tcm (2.20+TSQD-7)
  command 'tt' from deb treetop (1.6.8-1)
  command 'ttx' from deb fonttools (4.29.1-2build1)
See 'snap info <snapname>' for additional versions.
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ cp file1.txt file2.txt
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ cat file1.txt file2.txt | sort | uniq
pattern programming
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ cat >> file2.txt
hello
morning
evening
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ cat file1.txt file2.txt | sort | uniq
evening
hello
morning
pattern programming
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$  ls -l | grep "^d"
drwxr-xr-x 2 tanvee tanvee 4096 Mar  9 10:04 mydir
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ grep -r "pattern" file2.txt
pattern programming
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ cat file1.txt file2.txt | sort | uniq –d
uniq: –d: No such file or directory
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ cat file1.txt file2.txt | sort | uniq –d
uniq: –d: No such file or directory
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ touch file.txt
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ chmod 644 file.txt
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ ls -al
total 32
drwxr-xr-x 3 tanvee tanvee 4096 Mar  9 10:05 .
drwxr-xr-x 3 tanvee tanvee 4096 Mar  9 09:50 ..
-rw-r--r-- 1 tanvee tanvee   12 Mar  9 09:47 Part1.sh
-rw-r--r-- 1 tanvee tanvee    0 Mar  9 10:13 file.txt
-rw-r--r-- 1 tanvee tanvee   20 Mar  9 09:55 file1.txt
-rw-r--r-- 1 tanvee tanvee   20 Mar  9 10:05 file2.
-rw-r--r-- 1 tanvee tanvee   42 Mar  9 10:06 file2.txt
drwxr-xr-x 2 tanvee tanvee 4096 Mar  9 10:04 mydir
-rwxr-xr-x 1 tanvee tanvee   40 Mar  9 09:52 script.sh
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ cp -r file2.txt file.txt
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ cat file.txt
pattern programming
hello
morning
evening
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ find hello "*.txt"
find: ‘hello’: No such file or directory
find: ‘*.txt’: No such file or directory
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ man find
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ find ./Assignment2 -name "*.txt"
find: ‘./Assignment2’: No such file or directory
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ cd ..
tanvee@LAPTOP-2EIP57DT:~/ShellProgram$ find ./Assignment2 -name "*.txt"
./Assignment2/mydir/file.txt
./Assignment2/file1.txt
./Assignment2/file.txt
./Assignment2/file2.txt
tanvee@LAPTOP-2EIP57DT:~/ShellProgram$ cd Assignment2
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ chmod u+x file.txt
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ ls -al
total 36
drwxr-xr-x 3 tanvee tanvee 4096 Mar  9 10:05 .
drwxr-xr-x 3 tanvee tanvee 4096 Mar  9 09:50 ..
-rw-r--r-- 1 tanvee tanvee   12 Mar  9 09:47 Part1.sh
-rwxr--r-- 1 tanvee tanvee   42 Mar  9 10:14 file.txt
-rw-r--r-- 1 tanvee tanvee   20 Mar  9 09:55 file1.txt
-rw-r--r-- 1 tanvee tanvee   20 Mar  9 10:05 file2.
-rw-r--r-- 1 tanvee tanvee   42 Mar  9 10:06 file2.txt
drwxr-xr-x 2 tanvee tanvee 4096 Mar  9 10:04 mydir
-rwxr-xr-x 1 tanvee tanvee   40 Mar  9 09:52 script.sh
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ echo $PATH
/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/usr/lib/wsl/lib:/mnt/c/Program Files/Common Files/Oracle/Java/javapath:/mnt/c/oraclexe/app/oracle/product/11.2.0/server/bin:/mnt/c/Windows/system32:/mnt/c/Windows:/mnt/c/Windows/System32/Wbem:/mnt/c/Windows/System32/WindowsPowerShell/v1.0/:/mnt/c/Windows/System32/OpenSSH/:/mnt/c/Program Files/Microsoft VS Code/bin:/mnt/c/MinGW/bin:/mnt/c/Program Files/Git/cmd:/mnt/c/Program Files/Java/jdk-21/bin:/mnt/c/Program Files/dotnet/:/mnt/c/Users/Tejas Eknath Naik/AppData/Local/Programs/Python/Launcher/:/mnt/c/Users/Tejas Eknath Naik/AppData/Local/Microsoft/WindowsApps:/snap/bin




PART B


Identify True or False: 

1. ls is used to list files and directories in a directory. => TRUE 

2. mv is used to move files and directories. => TRUE

3. cd is used to copy files and directories. => FALSE

4. pwd stands for "print working directory" and displays the current directory. => TRUE

5. grep is used to search for patterns in files. => TRUE

6. chmod 755 file.txt gives read, write, and execute permissions to the owner, and read and execute 
permissions to group and others. => TRUE

7. mkdir -p directory1/directory2 creates nested directories, creating directory2 inside directory1 
if directory1 does not exist. => TRUE

8. rm -rf file.txt deletes a file forcefully without confirmation. => TRUE

Identify the Incorrect Commands: 
1. chmodx is used to change file permissions. => chmod

2. cpy is used to copy files and directories. => cp

3. mkfile is used to create a new file. => mkdir,cat,touch


4. catx is used to concatenate files. => false

5. rn is used to rename files. => mv



PART C

Question 1: Write a shell script that prints "Hello, World!" to the terminal. 

tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ cat Partc.sh
#!/bin/bash
echo "Hello, World!"

---------------------------------------------------------------------------------------------
Question 2: Declare a variable named "name" and assign the value "CDAC Mumbai" to it. Print the 
value of the variable

tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ cat C2.sh
#!/bin/bash
name="CDAC MUMBAI"
echo $name
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ ./C2.sh
CDAC MUMBAI

--------------------------------------------------------------------------------------------
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ cat C3.sh
#!/bin/bash
read number
echo $number
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ ./C3.sh
3
3

---------------------------------------------------------------------------------------------
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ cat C4.sh
#!/bin/bash
a=5
b=3
((sum=$a+$b))
echo $sum
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ ./C4.sh
8

---------------------------------------------------------------------------------------------

tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ cat C5.sh
#!/bin/bash
read number
if [[ `expr $number % 2` == 0 ]]
then
        echo "Even"
else
        echo "Odd"
fi
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ ./C5.sh
2
Even

------------------------------------------------------------------------------------------

tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ cat C6.sh
#!/bin/bash
for (( i=1; i<=5; i++ ))
do
        echo $i
done

tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ ./c6.sh
-bash: ./c6.sh: No such file or directory
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ ./C6.sh
1
2
3
4
5

----------------------------------------------------------------------------------------

tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ cat C7.sh
#!/bin/bash
i=1
while [[ i -le 5 ]]
do
        echo $i
        i=$(($i+1))
done
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ ./C7.sh
1
2
3
4
5

------------------------------------------------------------------------------------------

tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ vi C8.sh
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ pwd
/home/tanvee/ShellProgram/Assignment2
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ vi C8.sh
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ vi C8.sh
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ chmod +x C8.sh
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ ./C8.sh
File exist
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ cat C8.sh
#!/bin/bash
file="/home/tanvee/ShellProgram/Assignment2/C7.sh"
if test -f "$file"
then
        echo "File exist"
else
        echo "File does not exist"
fi
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ vi C8.sh
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ ./C8.sh
File exist
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ vi C8.sh
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ ./C8.sh
File does not exist

-------------------------------------------------------------------------------------------


tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ vi C9.sh
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ chmod +x C9.sh
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ ./C9.sh
Enter the Number :
4
./C9.sh: line 9: syntax error: unexpected end of file
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ vi C9.sh
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ ./C9.sh
Enter the Number :
4
Number is smaller that 10

#!/bin/bash
echo "Enter the Number : "
read n
if [[ $n -ge 10 ]]
then
        echo "Number is greater that 10"
else
        echo "Number is smaller that 10"
fi

----------------------------------------------------------------------------------------


tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ vi C10.sh
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ ./C10.sh
1 x 1 = 1
1 x 2 = 2
1 x 3 = 3
1 x 4 = 4
1 x 5 = 5
1 x 6 = 6
1 x 7 = 7
1 x 8 = 8
1 x 9 = 9
1 x 10 = 10

2 x 1 = 2
2 x 2 = 4
2 x 3 = 6
2 x 4 = 8
2 x 5 = 10
2 x 6 = 12
2 x 7 = 14
2 x 8 = 16
2 x 9 = 18
2 x 10 = 20

3 x 1 = 3
3 x 2 = 6
3 x 3 = 9
3 x 4 = 12
3 x 5 = 15
3 x 6 = 18
3 x 7 = 21
3 x 8 = 24
3 x 9 = 27
3 x 10 = 30

4 x 1 = 4
4 x 2 = 8
4 x 3 = 12
4 x 4 = 16
4 x 5 = 20
4 x 6 = 24
4 x 7 = 28
4 x 8 = 32
4 x 9 = 36
4 x 10 = 40

5 x 1 = 5
5 x 2 = 10
5 x 3 = 15
5 x 4 = 20
5 x 5 = 25
5 x 6 = 30
5 x 7 = 35
5 x 8 = 40
5 x 9 = 45
5 x 10 = 50

#!/bin/bash
n=5
for (( i=1; i<=5; i++ ))
do
        for (( j=1; j<=10; j++ ))
        do
                ((mul=$i*$j))
                echo "$i x $j = $mul"
        done
        echo " "
done

-------------------------------------------------------------------------------------------------


tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ vi C11.sh
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ ./C11.sh
enter number
2
number = 2
enter number
-2
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ ./C11.sh
enter number
3
number = 3
enter number
6
number = 6
enter number
10000
number = 10000
enter number
0
number = 0
enter number
-22
tanvee@LAPTOP-2EIP57DT:~/ShellProgram/Assignment2$ cat C11.sh
#!/bin/bash
while [[ i -ge 0 ]]
do
        echo "enter number"
        read n
        if [[ $n -ge 0 ]]
        then
                echo "number = $n"
        else
                break;
        fi
done

-----------------------------------------------------------------------------------------



