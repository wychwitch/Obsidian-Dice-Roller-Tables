# Obsidian-Dice-Roller-Tables
This is a collection of Dice Roller Tables (and some Rant generators) that I use to run my DND campaigns! Feel free to fork, remix, and tweak to suit your needs! I'm also open to pull requests!

**Please update to the latest version of the dice roller, buttons, and Rant plugins to be able to use these pages!**

It's also recommended that you turn off *Display formula with results*, *Display Lookup Table Roll*, and *Show Dice Button* for maximum compatibility!

## Example of NPC Generator
![2hDw43Oiub](https://user-images.githubusercontent.com/1291820/142545127-0690300d-1f55-4563-a523-0a2e715d483f.gif)

## Example of Rant NPC Generator
![Obsidian_v0MHEjeV14](https://user-images.githubusercontent.com/1291820/153722698-839ef87a-3cd7-4fb6-be8a-6dfe0b503b1f.gif)


## Overview
At the moment I have the following pages:
- [[New NPC Generator]]
  - The new npc generator utilizing the powers of rant! Since rant is still in development, an update may temporarily break things! I'll try to update as soon as possible
- [[_Example Generators]]
	- Go here to see some of the implementations of the tables! Right now it's only a NPC generator!
- [[Misc Dice Tables]]
	- A collection of tables that don't belong elsewhere
- [[Name Dice Tables]]
	- All the tables relating to names! Feel free to go in here and add tweak some!
- [[NPC Dice Tables]]
	- All tables related to NPC generation! 
- [[Race Dice Tables]]
	- The tables related to race generation! This is especially modified for my campaign, so feel free to mess around with this and shuffle some other races in or out!
- [[Tarot Dice Tables]]
	- Tarot, but in dice form! I use this a lot to get the vibe of a place, or for associating it to a character. 


## Optional Scripts

### txt2dice
If you're interested, I also wrote a small script called txt2dice to convert any txt file list (with each item on a newline) in python3! Save the below code and run it as `py path/to/txt2dice.py path/to/file-name.txt`

```python
import argparse


parser = argparse.ArgumentParser(description='Converts a list into a diceroller-formatted md table', prog='txt2dice')
parser.add_argument('input', help='The file to convert to markdown!')

parser.add_argument('--output', '-o', help='The name of the file to write to! Warning: This WILL overwrite any file that exists already.Default is txt2dice-output.md', default='txt2dice-output.md', required=False)
parser.add_argument('--title', '-t', help='The name of the table you will generate! It will also add it as a block id.', default='Table', required=False)

args = parser.parse_args()

listOfLines = []

mdTableBody = ""

mdTable = ""  

try:
  with open(f'{args.input}') as afile:
    listOfLines = afile.read().splitlines() 
except FileNotFoundError:
  print(f"Could not find {args.input}")

num = 1
for item in listOfLines:
  mdTableBody += f"\n|{num}|{item}|"
  num +=1

mdTableBody += f"\n^{args.title}\n"
mdtableHeader = f"""| dice: 1d{num-1} | {args.title}|
| --------- | ------------------- |"""

mdTable = mdtableHeader + mdTableBody

if args.output.endswith('.md'):
  text_file = open(f"{args.output}", "w")
  text_file.write(mdTable)
  text_file.close()
else:
  text_file = open(f"{args.output}.md", "w")
  text_file.write(mdTable)
  text_file.close()

print(f"Converted and saved to {args.output}!")
#print(mdTable)
```

```python
from random import randint
with open(f'name-list.txt') as afile:
    listOfLines = afile.read().splitlines() 
newnames = ""

for i in range (0,2000):
    newnames += listOfLines.pop(randint(0,len(listOfLines)-1)) + "\n"


text_file = open(f"narrowed-names.txt", "w")
text_file.write(newnames)
text_file.close()
```

### narrow-down-names
This is a quick and dirty program to make that **long** list of names into a much smaller list!

Here it is, keep in mind the file names are hardcoded!

```python
from random import randint
with open(f'name-list.txt') as afile:
    listOfLines = afile.read().splitlines() 
newnames = ""

for i in range (0,2000):
    newnames += listOfLines.pop(randint(0,len(listOfLines)-1)) + "\n"


text_file = open(f"narrowed-names.txt", "w")
text_file.write(newnames)
text_file.close()
```
