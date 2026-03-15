# Bandit Learning Reflections

## Level 0-1
**What I learned:** How to use cat to read files and ./ to handle files with special characters in the name like -
**Struggled with:** Didn't know why cat - didn't work, learned that - means keyboard input to Linux

## Level 1-2
**What I learned:** Spaces in filenames confuse Linux because it thinks each word is a separate file
**Struggled with:** Didn't know about quotes to group filenames together

## Level 2-3
**What I learned:** Files starting with . are hidden from normal ls
**Struggled with:** Thought the directory was empty, needed ls -la to see hidden files

## Level 3-4
**What I learned:** file command tells you what type a file is without opening it
**Struggled with:** Tried to cat everything including directories

## Level 4-5
**What I learned:** find command searches for files by size, owner, group
**Struggled with:** Didn't know find existed, was going to check folders manually

## Level 5-6
**What I learned:** find / searches the whole server, lots of permission denied is normal
**Struggled with:** Too much output, had to spot the one result that wasn't an error

## Level 6-7
**What I learned:** grep searches for a word inside a file
**Struggled with:** Nothing major here, picked it up quickly

## Level 7-8
**What I learned:** Piping sort into uniq -u finds lines that appear only once
**Struggled with:** Didn't know what uniq -u did or why you need to sort first

## Level 8-9
**What I learned:** strings extracts human readable text from binary files
**Struggled with:** Didn't know binary files cant be read with cat

## Level 9-10
**What I learned:** base64 -d decodes base64 encoded data, -d flag means decode
**Struggled with:** Had to use man base64 to find the right flag

## Level 10-11
**What I learned:** tr command does character translation, ROT13 shifts letters 13 positions
**Struggled with:** Had no idea what ROT13 was before this level

## Level 11-12
**What I learned:** xxd -r converts hexdump back to binary, files can be compressed multiple times
**Struggled with:** This was the hardest level so far. Had to repeatedly check file type and decompress with different tools - gzip, bzip2 and tar all work differently
**Key commands learned:**
- gzip -d file.gz
- bzip2 -d file.bz2  
- tar xf file.tar

## Overall Reflection
The biggest thing I learned is to always read error messages carefully and use the file command before assuming what something is. I found piping the hardest concept at first but it makes sense now - you chain commands together so the output of one feeds into the next.
