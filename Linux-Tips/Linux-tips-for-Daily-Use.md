# Linux-Tips

### Table of Contents
---

| No. | Topic                                                                   |
| --- | ----------------------------------------------------------------------- |
| 1   | [**Text columns adding , filter and rearrange using Linux commands**](#user-information)                               |
| 2   | [**Extracting a images from pdf and converting into a video**](#file)         |
| 3   | [**File**](#file)                               |


 1 .**Text column**

```
 192.168.16.87	LABp34
[Need to be filter the last part of the ip 87]

cut -d "." -f4 new >first
output:
87	LABp34

[I need to include the PL and A to the 2nd and 3rd column]
[So i add the number first and i replaced the number to the 'PL']

cat first | nl -n 'rz' -w 2 > file
DIsplays with number

:%s/^[0-9]\+/IN/
replace the number with IN

[Do it 2 times because of IN and PL should be entererd]

'Everything is done only need to the columns arranged'

So using awk we can arrange the columns and give the space to the columns
awk '{print $1 "\t" $2 "\t" $3 "\t" $4}' input.txt > output.txt

Atlast i want to add the .a2d to the last column of the last line
awk '{$4 = $4 ".a2d"; print}' input.txt > output.txt

[It shows the output correctly]
  ```
---
2. **Extracting a images from pdf and converting into a video**

Install the necessary
```
sudo apt-get install poppler-utils
```
```
sudo apt install ffmpeg
```

It Extracts the page from 1 to 50
```
pdftoppm -f 1 -l 50 demo.pdf page
```

Converts the ppm files to png extension
```
mogrify -format png page-*.ppm
```

After converting to png format remove ppm files
```
rm *.ppm
```

Converting png images to video with 3 seconds delay
```
ffmpeg -framerate 1/3 -pattern_type glob -i '*.png' -vf "scale=1242:1754" -c:v libx264 -r 30 -pix_fmt yuv420p output.mp4
```


---


