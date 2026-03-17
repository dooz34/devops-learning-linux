# Bandit Learning Reflections

## Level 0-1
**What I learned:** How to use cat to read files and ./ to handle files with special characters in the name like -

## Level 1-2
**What I learned:** Spaces in filenames confuse Linux because it thinks each word is a separate file. Use quotes to group filenames together

## Level 2-3
**What I learned:** Files starting with . are hidden from normal ls. Use ls -la to see all files including hidden ones

## Level 3-4
**What I learned:** The file command tells you what type a file is without opening it. You cannot cat a directory

## Level 4-5
**What I learned:** The find command searches for files by size, owner, group across directories automatically

## Level 5-6
**What I learned:** find / searches the whole server. Lots of permission denied errors is normal - look for the one result that isn't an error

## Level 6-7
**What I learned:** grep searches for a specific word inside a file

## Level 7-8
**What I learned:** Piping sort into uniq -u finds lines that appear only once. You must sort first before uniq can work properly

## Level 8-9
**What I learned:** strings extracts human readable text from binary files. Binary files cannot be read with cat

## Level 9-10
**What I learned:** base64 -d decodes base64 encoded data. The -d flag means decode. Use man to find flags you don't know

## Level 10-11
**What I learned:** tr command does character translation. ROT13 shifts every letter 13 positions forward in the alphabet

## Level 11-12
**What I learned:** xxd -r converts hexdump back to binary. Files can be compressed multiple times with different tools
**Key commands:**
- gzip -d file.gz
- bzip2 -d file.bz2
- tar xf file.tar

## Level 12-13
**What I learned:** SSH private keys can be used instead of passwords to authenticate. The -i flag specifies the key file. chmod 400 sets correct key permissions

## Level 13-14
**What I learned:** nc (netcat) connects to a TCP port and sends data to it. You can pipe a password directly into it using echo

## Level 14-15
**What I learned:** openssl s_client connects to a port using SSL/TLS encryption. Some services require encrypted connections. The -quiet flag stops extra output

## Level 15-16
**What I learned:** nmap scans ports to find what services are running. Use -sV to detect service types. Scan ranges of ports to find the right one

## Level 16-17
**What I learned:** diff compares two files line by line and shows what changed. The < line is old and the > line is new

## Level 17-18
**What I learned:** You can run a command directly over SSH without logging in interactively by appending it to the SSH command. This bypasses shell startup scripts

## Level 18-19
**What I learned:** Setuid binaries run with the permissions of their owner not the person running them. This allows controlled privilege escalation

## Level 19-20
**What I learned:** You can create a local listener with nc -l and have another process connect to it. Some tasks require coordinating two terminal sessions at the same time

## Takeaways

Completing all 20 levels of Bandit has been one of the most hands-on learning experiences I've had. At the start I didn't know basic commands like cat and ls properly. By the end I was using netcat, openssl and nmap to interact with network services.

The hardest parts were level 12 where I had to decompress a file multiple times using different tools, and level 13 where I had to transfer an SSH key from the server to my local machine. Both took a lot of trial and error and taught me to read error messages properly instead of guessing.

The biggest thing I struggled with overall was piping. At first I didn't understand why you would chain commands together but now I can see how powerful it is — combining sort, uniq, grep and strings lets you do things that would take ages manually.

Going forward I want to get faster at recognising which command to use in each situation without needing to look it up. I also want to understand networking concepts like ports and SSL better as these came up a lot in the later levels and are clearly important for DevOps work.
