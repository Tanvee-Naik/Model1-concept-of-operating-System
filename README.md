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
