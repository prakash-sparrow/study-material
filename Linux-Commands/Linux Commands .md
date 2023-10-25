# Linux Commands 
### Table of Contents
---
| No. | Topic                                                                                                               | No | Topic
| --- | -----------------------------------------------------------------------                                             |----| ----------------------------
| 1   | [*cat*](https://github.com/prakash-sparrow/study-material/blob/main/Linux-Commands/Linux%20Commands%20.md#cat-commands)         | 16 | [*sort / Uniq*](https://github.com/prakash-sparrow/study-material/blob/main/Linux-Commands/Linux%20Commands%20.md#sort--uniq-commands)
| 2   | [*tr*](https://github.com/prakash-sparrow/study-material/blob/main/Linux-Commands/Linux%20Commands%20.md#tr-commands)           | 17 | [*tar*](https://github.com/prakash-sparrow/study-material/blob/main/Linux-Commands/Linux%20Commands%20.md#tar-commands)
| 3   | [*ls*](https://github.com/prakash-sparrow/study-material/blob/main/Linux-Commands/Linux%20Commands%20.md#ls-commands)           | 18 | [*gzip*](https://github.com/prakash-sparrow/study-material/blob/main/Linux-Commands/Linux%20Commands%20.md#gzip-commands)
| 4   | [*echo*](https://github.com/prakash-sparrow/study-material/blob/main/Linux-Commands/Linux%20Commands%20.md#echo-commands)       | 19 | [*split*](https://github.com/prakash-sparrow/study-material/blob/main/Linux-Commands/Linux%20Commands%20.md#split-commands)
| 5   | [*find*](https://github.com/prakash-sparrow/study-material/blob/main/Linux-Commands/Linux%20Commands%20.md#find-commands)       | 20 | [*export*](https://github.com/prakash-sparrow/study-material/blob/main/Linux-Commands/Linux%20Commands%20.md#export-commands)
| 6   | [*python*](https://github.com/prakash-sparrow/study-material/blob/main/Linux-Commands/Linux%20Commands%20.md#python-commands)   | 21 | [*apropos*](https://github.com/prakash-sparrow/study-material/blob/main/Linux-Commands/Linux%20Commands%20.md#apropos-commands)
| 7   | [*sed*](https://github.com/prakash-sparrow/study-material/blob/main/Linux-Commands/Linux%20Commands%20.md#sed-commands)         | 22 | [*nl*](https://github.com/prakash-sparrow/study-material/blob/main/Linux-Commands/Linux%20Commands%20.md#nl-commands)
| 8   | [*cut*](https://github.com/prakash-sparrow/study-material/blob/main/Linux-Commands/Linux%20Commands%20.md#cut-commmands)        | 23 | [*Bash*](https://github.com/prakash-sparrow/study-material/blob/main/Linux-Commands/Linux%20Commands%20.md#bash-commands)
| 9   | [*cal*](https://github.com/prakash-sparrow/study-material/blob/main/Linux-Commands/Linux%20Commands%20.md#cal-commands)         | 24 | [*shred*](https://github.com/prakash-sparrow/study-material/blob/main/Linux-Commands/Linux%20Commands%20.md#shred-commands)
| 10  | [*less*](https://github.com/prakash-sparrow/study-material/blob/main/Linux-Commands/Linux%20Commands%20.md#less-commands)       | 25 | [*apt*](https://github.com/prakash-sparrow/study-material/blob/main/Linux-Commands/Linux%20Commands%20.md#apt-commands)
| 11  | [*nano*](https://github.com/prakash-sparrow/study-material/blob/main/Linux-Commands/Linux%20Commands%20.md#nano-commands)       | 26 | [*Yt-dlp*](https://github.com/prakash-sparrow/study-material/blob/main/Linux-Commands/Linux%20Commands%20.md#yt-dlp-coammands)
| 12  | [*tmux*](https://github.com/prakash-sparrow/study-material/blob/main/Linux-Commands/Linux%20Commands%20.md#tmux-commands)       | 27 | [*tac*](https://github.com/prakash-sparrow/study-material/blob/main/Linux-Commands/Linux%20Commands%20.md#tac-commands)
| 13  | [*curl*](https://github.com/prakash-sparrow/study-material/blob/main/Linux-Commands/Linux%20Commands%20.md#curl-commands)       | 28 | [*sha256*](https://github.com/prakash-sparrow/study-material/blob/main/Linux-Commands/Linux%20Commands%20.md#sha256-command)
| 14  | [*awk*](https://github.com/prakash-sparrow/study-material/blob/main/Linux-Commands/Linux%20Commands%20.md#awk-commands)         | 29 | [*zip*](https://github.com/prakash-sparrow/study-material/blob/main/Linux-Commands/Linux%20Commands%20.md#zip-command)
| 15  | [*grep*](https://github.com/prakash-sparrow/study-material/blob/main/Linux-Commands/Linux%20Commands%20.md#grep-commands)       | 30 | [*common-command*](https://github.com/prakash-sparrow/study-material/blob/main/Linux-Commands/Linux%20Commands%20.md#common-linux-commands)


| No. | Topic                                                                                                               | No | Topic
| --- | -----------------------------------------------------------------------                                             |----| ----------------------------
| 1   | [*tee*](https://github.com/prakash-sparrow/study-material/blob/main/Linux-Commands/Linux%20Commands%20.md#tee-commands)  | 2 | [*timeout*](https://github.com/prakash-sparrow/study-material/blob/main/Linux-Commands/Linux%20Commands%20.md#timeout-commands)
| 3   | [*column*](https://github.com/prakash-sparrow/study-material/blob/main/Linux-Commands/Linux%20Commands%20.md#column-commands)  | 4 | [*shuf*](https://github.com/prakash-sparrow/study-material/blob/main/Linux-Commands/Linux%20Commands%20.md#shuf-commands)
| 5   | [*xargs*](https://github.com/prakash-sparrow/study-material/blob/main/Linux-Commands/Linux%20Commands%20.md#xargs-commands)	  | 6 | [*command*]()



### Cat Commands
```
$ cat > demofile.txt
    To type the content into the terminal
    type
    and CTRL + C to quit and save

$ cat << EOF > anything.txt
    type the content when you want to end give EOF
    Type EOF to end the and save the file

$ cat << STOP > demo.txt
    type the content when you want to end give EOF
    Type EOF to end the and save the file
```

### Tr Commands

```
$ tr A-Z a-z > songs.txt
    Convert a file to all lower-case
```

### ls Commands

```
$ ls ..
    Shows the file one folder back

$ ls ../..
    Shows the file two folder back

$ ls -1
    It will show the files in Vertical order
```

### Echo Commands

```
$ echo {1..9}
    Prints 1 to 9 numbers

$ echo {a..z}
    Print a to z alphabetical letters

$ echo *.txt
    Result the all text files in current folder 
    Same result as ls *.txt
```

### Find Commands

```
$ find . -name *.gz -delete
    It deletes the *.gz files

$ find . -type f -name "file[1-9]" -delete
    It deletes the file1 to file9

$ find /etc/ -type f 2> /dev/null
    It will find the files and if some error happend it will ommited

$ find /etc/ -type f 1> ~/results.txt 2> ~/errors.txt
    [or]
$ find /etc/ -type f >results.txt 2> errors.txt
    It will find the files and result will be save in results.txt if errors occurs that will save in errors.txt

$ find /etc/ -type f >>results.txt 2>> errors.txt
    It will find the results and error save in seperate file and >> overwrite the content

SEARCH THE FILES COPY AND MOVE TO ANOTHER FOLDER

$ find . -type f -name "*.mp4" -exec mv {} /c/users/jp/download/videos \;
$ find . -name "*.epub" -exec cp {} ../folder/ \;

REMOVING FILES 

$ find /home/foo -type f -name "*.txt" -exec rm {} \;
    remove all the files that has .txt

```

### Python Commands

```
$ python -m http.server 8989
    To start the python server
```

### Sed Commands

```
$ sed 's/..$//'
    THis is for remove last two words
    
$ sed 's/.$//'
    This is for remove last one words
    
$ sed 's/types/Mubi/g' filename.txt
    /g for global
    It will replace types to Mubi in all words

$ sed -i 's/types/Mubi/g' filename.txt
    It Will Insert the TEXT into the file

$ sed -i 's/Mubi//g' com.txt 
    It will Search the Mubi and Replace with EMPTY 

$ sed '/Sed/d' com.txt 
    It will find the word sed and /d for delete and delete it

$ sed '/^$/d' com.txt
    It will find the empty line and delete it ^ for all $ for nothing

$ sed '1d' file.txt
    It will delete the first line

$ sed '1,2d' file.txt
    It will delete the first and Second Line

$ sed 's/\t/ /g' com.txt 
    It will remove the \t for TAB in text
    
$ sed -n 5,6p filename.txt
    It will grep the 5,6 line in the file
    
$ sed 2,3d filename.txt 
    It will verbose that is it will print opposite to 2,3 line
    
$ sed G com.txt 
    It will give space for every line
```

### Cut Commmands

```
$ cut -c 6-
    This is for remove first 6 character

$ echo "This is a line" | cut -c 1-10
    Displays First 10 charcter 

$ cut -d ' ' -f5
    Grab the 5th field

$ cat pratice.txt | cut -c2
    It will print Charcter two  (jason - 'a' will be printed)
    
$ cat pratice.txt | cut -c2,3
    It will print character 2,3 (jason - 'as' will be printed)

$ cat pratice.txt | cut -c2-8
    It will print character 2 to 8 ( theoneyinileo   -  'heoneyin' will be printed)

$ cut -c2- pratice.txt 
    It will print from 2nd charcter to last end

$ cat new1.txt | nl | cut -d'<' -f1
    It will cut the text after < and print with field 1 that is -f1
    
$ cut -c1-3 filename		-   List range of characters

$ cut -c1-3,6-8 filename	-   List specific range of characters

$ cut -b1-3 filename		-   List by byte size

$ cut -d: -f 6 /etc/passwd	-   List first 6th column separated by:

$ cut -d: -f 6-7 /etc/passed	-   List first 6 and 7th column separated by:

$ ls -l | cut -c2-4		-   Only print user permisson of files /dir
```

### Cal Commands

```
$ cal -y
    It will shows the current full year
    
$ cal 03 2023
    It will shows the particular date, month, year
```

### Less Commands

```
$ less /var/log/alternatives.log
    Shows the log files with less
Type -S for giving the clarity text
Move  RIGHT   --> or LEFT  <-- arrow to move
Type -N for giving the Nummbers to the line
```

### Nano Commands

```
Ctrl + x  +   Ctrl + E   ---> Open the Nano Editor
```

### Tmux Commands

```
Type tmux and enter into tmux window
tmux splitw   - To create a window Horizontally
tmux splitw -h  - To create a window Vertically

TO MOVE TO ANTOHER WINDOW
Press Ctrl + B and followed by UP Arrow or DOWN Arrow or LEFT Arrow or RIGHT Arrow

Ctrl + B and   <-- or  -->
```

### Curl Commands

```
$ curl ipinfo.me
    It will show the ip address and details of ISP

$ curl ifconfig.me
    It will show the only the ip address

$ curl ipinfo.me/192.168.86.91
    It will show the ip address all of the details

WEBSITE TO UPLOAD THE TEXT
$ cat textfile.txt | curl -F 'clbin=<' https://clbin.com
    It will provide the link

$ curl -F 'f:1=@aria.txt' ix.io
    It will provide the  link for the text file
```

### Awk Commands

```
$ ls -l | awk '{print $NF}'	
    Print the Last word of the file

$ awk '/Jerry/ {print}' file
    Search for a specific word

$ awk -F: '{print $1}' /etc/passed
    Ouput only 1st field of /etc/passwd

$ echo "hello" | awk '{$2="adam"; print $0}' 
    Replace words fields words

$ awk 'length($0) > 15' file
    Get lines that have more than 15 byte size

$ ls -l | awk '{if($9 == "sein") print  $0;}
    Get the field matching sein in /home/neo

$ ls -l | awk '{print NF}'
    Number of fields
```

### Grep Commands

```
grep -c the demo.txt		-	Search for a keyword and count

grep -i the demo.txt		-	Search for a keyword ignore case-sensitive

grep -n the file.txt		-	Display the matched lines and their line numbers

grep -v them file.txt		-	Display everything except opposite to the keywords

ls -l | grep Desktop		-	Grep the input

egrep -i "keyword|keyword" demo.txt	- Search for 2 Keywords
```

### Sort / Uniq Commands

```
sort file			-	Shorts file in alphabetical order

sort -n shuffled-numbers.txt    - 	It will arrange the shuffled number
	
sort -R .bashrc		        - 	randomly arrange the lines

sort -r file			-	Short in reverse alphabetical order

sor -k2 file			-	Sort by field number

uniq file			-	Removes Duplicates

sort file | uniq		-	Always sort first before using uniq their line numbers

sort file | uniq -c		-	Sort first then uniq and list count

sort file | uniq 0d		-	Only show repeated lines

sort -k2 -t$'\t' -n filename.txt
It will sort the second column of dob
the first column has two to three alphabetical names
the second has dob it has to sort in numberical order
so this commands help to order it

sort -k2 -t$'\t' -n filename.txt
Same in Reverse Order
```

### Tar Commands

```
tar cvf files.zip .		-	Create  tar file

tar xvf files.zip		-	Extracts tar file

tar tvf files.zip		-	Tables the content of the file
```

### Gzip Commands

```
gzip files.txt			-	It will create the file and overwritten

gzip -d files.txt		-	It will extract the files
```

### Split Commands 

```
$ cat demo.txt
    india
    japan
    france
    swiz

$ split -l 2 demo.txt sep
    ls
    sepa	sepb

$ cat sepa
    india 
    japan

$ cat sepb
    france 
    swiz
```

### Export Commands

```
$ export PS1="Hello World> "
    It will output the terminal as
    Hello World> 

$ export PS1="\u@\h \w> "
    u - Username
    h - hostname
    w - working directory
LAPTOP5BM@jp /Python >
```

### Apropos Commands

```
apropos   -  Search the manuel page and give the names and descriptions
ex:
apropos ffmpeg
apropos zip
apropos grep
```

### nl Commands

```
$ cat names.txt | nl -n 'rz' -w 2
    Gives the number

$ ls|nl -n'rz' -s"_" -w3
    List of name the files with numbers
```

### Bash Commands

```
TO run the files.txt in terminal
$ cat command-file
ls -lah

use
$ bash command-file
It will execute in the terminal
```

### Shred Commands

```
$ shred -uvz -n 10 filename
    securely deletes and overwrites the contents of the file difficult to recover
```

### apt commands

```
$ apt list --installed
    To check how many programs installed
```

### Yt-dlp Coammands

```
$ yt-dlp --write-sub --write-auto-sub --skip-download "link"
    To download the Youtube video subtitles Only
```

### Tac commands

```
$ tac filename.txt
    It will reverse the text of the file last to first
```

### sha256 Command

```
$ sha256sum clbin.txt
    It will generate the sha256 uniq code
```
### Zip Command

```
Zip file password create

$ zipcloak filename.zip
    Enter password:
    verify password:
It will Encrypt the file with given password
```

### Common Linux Commands
```
$ cat web.txt | grep .jpg | awk '{print }'|sed 's/.$//' | cut -c 6- > final.txt

$ ls | xargs du -h *

Generating Random number
$ head 3 /dev/urandom
$ head 3 /dev/urandom | tr -cd '[:print:]'
    d -delete
    c -compliment
    print - print the character
    
man -k .  - It list all the man pages

TO delete the blank unwanted lines in vim
/g/^$/d

$ sort -k2 -t$'\t' -n filename.txt
    It will sort the second column of dob
    the first column has two to three alphabetical names
    the second has dob it has to sort in numberical order
    so this commands help to order it

sort -k2 -t$'\t' -n filename.txt
    Same in Reverse Order

To convert man page to pdf
Requirements
	ps2pdf
	ghostscript
$ man -t ls | ps2pdf - ls-manual.pdf

```



### tee Commands
```
$ ls -lah | tee output.txt
	It will show the output of the command and store the output in the output.txt

$ ls -lah desktop-fi 2>&1 | tee output.txt
	In this case "desktop-fi" directory is not available
	It will shows the error, in tee command it store only the output not error
	in case to store the output + error we need to use 2>&1 
		Example
			ls non_existent_directory 2>&1 | tee error_output.txt

$ ls -lah | tee -a output.txt
	In this case output.txt file is available -a is to append means overwrite the file

```

### timeout Commands

```
$ timeout 5s ping 127.0.0.1
	It will execute the ping command for 5 seconds and it will automatically exit

$ timeout 60s vim filename.txt
	It will exit the vim in 60 seconds

$ timeout 2m ./some_script.sh
	It will execute the script file for 2minutes

$ timeout 30s kill 1234
	It will kill the process after 30 seconds
```


### column Commands

```
$ cat newfile.txt
01 IRONMAN Avengers
02 SPider-man Avengers
03 X-men Wolverine

$ cat newfile.txt | column -t
01  IRONMAN     Avengers
02  SPider-man  Avengers
03  X-men       Wolverine

$ cat newfile.txt | column -t -s " "
01  IRONMAN     Avengers
02  SPider-man  Avengers
03  X-men       Wolverine

$ cat newfile.txt | column -t  -s " " -N "ONE,TWO,THREE"
ONE  TWO         THREE
01   IRONMAN     Avengers
02   SPider-man  Avengers
03   X-men       Wolverine

$ cat newfile.txt | column -t  -s " " -N "ONE,TWO,THREE" -o "| "
ONE| TWO       | THREE
01 | IRONMAN   | Avengers
02 | SPider-man| Avengers
03 | X-men     | Wolverine
```

### shuf Commands
```
$ seq 10 | shuf
	It will shuffle and give random numbers

$ seq 10 | shuf -n 1
	Generate 1 random number from 1 to 10

$ seq 10 > test.txt
	shuf test.txt -o shuffled-numbers.txt
	Generate 10 random number and shuffled the output to text file

$ shuf -n 3 -i 1-10 --repeat
	[or]
$ shuf -n 3 -i 1-10
	It will shuffle the number from 1 to 10 and gives the 3 numbers shuffled
```

### xargs Commands
```
$ ls |xargs  ls
	It will list the content and xargs with ls will ls the list of content
	for every output like ls -R

$ cut -d: -f1 < /etc/passwd | sort | xargs
	It will cut the first field 

$ ls | xargs -I {} echo "/home/files/{}"
	[or]
$ ls | xargs -I xxxxx echo "/home/files/xxxxx"
	It will add the text /home/files/{ls files will be included here}

$ seq 1000 | xargs -I {} touch {}.txt
	This command create 1000 files named 1.txt 2.txt upto 1000.txt

$ ls | cut -d. -f1 | xargs -I {} mv {}.txt {}.text
	It will cut the first field of the listed names and move the .txt extension to .text extension

$ find /home/foo -type f -name "*.txt" | xargs rm
	This command find the .txt files in the particular directory and removes the files 

```
