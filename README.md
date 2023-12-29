# command-line-arguments-to-count-word
## AIM:
To write a python program for getting the word count from the contents of a file using command line arguments.
## EQUIPEMENT'S REQUIRED: 
PC
Anaconda - Python 3.7
## ALGORITHM: 
### Step 1:
Import sys module.
### Step 2: 
 Open the file with sys.argv[1].
### Step 3: 
Use the for loop to select the content in file.
### Step 4:  
Use split function to to separate the file content into words or strings.
### Step 5: 
Count the length of the words using len.
### Step 6: 
Print the number of words.
## PROGRAM:
```
#To write a python program for getting the word count from the contents of a file using command line arguments.
#Developed by:Arikatla Hari Veera Prasad
#Register Number:212223240014
import sys
count = {}
total_count = 0
with open(sys.argv[1], 'r') as f:
    for line in f:
        for word in line.split():
            if word not in count:
                count[word] = 1
            else:
                count[word] += 1
            total_count += 1
print(count)
print(f"\nTotal word count: {total_count}")

```
### OUTPUT:
![image](https://github.com/Hariveeraprasad-2006/command-line-arguments-to-count-word/assets/145049988/f15c3a78-259a-45f7-ab0e-a4aa5cd9ea28)
## RESULT:
Thus the program is written to find the word count from the contents of a file using command line arguments.
