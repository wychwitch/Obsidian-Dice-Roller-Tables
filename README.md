# Obsidian-Dice-Roller-Tables
This is a collection of Dice Roller Tables that I use to run my DND campaigns! Feel free to fork, remix, and tweak to suit your needs!

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
