# Linux Commands 
### Table of Contents
---
| No. | Topic                                                                   |
| --- | ----------------------------------------------------------------------- |
| 1   | [*cat*](https://github.com/prakash-sparrow/study-material/blob/main/Linux-Commands/newfile.md#cat-commands)
 
### Common Linux Commands
```
$ cat web.txt | grep .jpg | awk '{print }'|sed 's/.$//' | cut -c 6- > final.txt
$ ls | xargs du -h *
```
 
 
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

### tr Commands

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

```

### echo Commands

```
$ echo {1..9}
    Prints 1 to 9 numbers
$ echo {a..z}
    Print a to z alphabetical letters
$ echo *.txt
    Result the all text files in current folder 
    Same result as ls *.txt
```

### find Commands

```
$ find . -name *.gz -delete
    It deletes the *.gz files
$ find . -type f -name "file[1-9]" -delete
    It deltes the file1 to file9
```

### python Commands

```
$ python -m http.server 8989
    To start the python server
```

### sed Commands

```
$ sed 's/..$//'
    THis is for remove last two words
$ sed 's/.$//'
    This is for remove last one words
```


### Cut Commmands

```
$ cut -c 6-
    THis is for remove first 6 character
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

$ cut -c1-3,6-8 filename		-   List specific range of characters

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
sort file			    -	Shorts file in alphabetical order

sort -r file			-	Short in reverse alphabetical order

sor -k2 file			-	Sort by field number

uniq file			    -	Removes Duplicates

sort file | uniq		-	Always sort first before using uniq their line numbers

sort file | uniq -c		-	Sort first then uniq and list count

sort file | uniq 0d		-	Only show repeated lines

```


