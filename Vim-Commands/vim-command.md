# Vim Commands

### Nomal Mode :

| Commands  | Explanation                                                                     |
|-----------|---------------------------------------------------------------------|
| ddp |  Delete the line and paste in next line [swapping]         
| di" |  Delete the words inside the "" [double quotes]
| yi" |  Copy the text inside "" [double quotes]
| ggdG |  Deletes the entire document
| gg | Go to first line fo the document
| dG | Deltes the lines after the cursor
| x  | To delete the character
| dw | To delete the word
| dd and p |  - simply it acts as copy paste the line dd for which line you want to |
|          | - p for which |
|	   | - line you paste|


### Insert Mode :
| Commands  |   Explanation                                                     |
|-----------|---------------------------------------------------------------------|				
| ctrl + w |  TO delete the word in INSERT Mode |
| ctrl + h | TO delte the single character |
| Ctrl + u |  Deltes the entire line before my cursor |
| shift + m |   Places the cursor in middle of the vim document |
| shift + l |  Places the cursor in low of the vim document |
|shift + h  |  Places the cursor in high of the vim document |
| Ctrl + u |  Move the document up |
| ctrl + d |  Move the document down |

### Command Mode : 
|Commands  |   Explanation                                                     |
|-----------|---------------------------------------------------------------------|	
| :set spell   | For check the spelling in the document |
| :set nospell | For turn of the spell |
| :set spell!  | For turn of the spell |
| :/word/m$	   | It will find the word and move to the last line |
|:10,43>	   | - Indenting the content of lines |
|		   | - (or) It will give the space of 1 TAB before line start |
|		   | - Punctuatuion |
|:ab lol lot of laugh | - When you type lol again it will automatically fill the rest of the sentence |
|		      | - ctrl + v to stop filling |
| /g/^$/       | To delete a unwanted lines in vim |
| :g/^\s*$/d   | his removes empty lines and that have zero or more whitespace characters (\s*) |
|:read !date | It will apply the date command |It will place the date text in 12th line |
| :12read !date | It will place the date text in 12th line |
| :$read !ls    | It will list the files names in last line |
| :%s/onefile/secondfile/g | It will replace teh 'onefile' text to 'secondfile' globally |
| :10,20s/991/500/g | It will repalce the 991 to 500 from line number 10 to 20 |


### Visual Mode
|Commands  |   Explanation                                                     |
|-----------|---------------------------------------------------------------------|	
|Ctrl +v  | For entering into visual mode and select the text type d for delete |
|ctrl +v  | * [Adding double quotes]Select the text like 10j it will select the first text|
|		  | * For entering command mode|
|:'<,'>  norm I"demo" | * norm for normal mode I for Insert and the text will appear one selected line|

