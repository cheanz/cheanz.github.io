# cut
## cut file
cut 
# wc : word count

# searching 
## `*"he“*`
## grep: text searching tool
```bash
grep -v "leo" /etc/passwd #反查
grep -n leo /etc/passwd #第几行
grep -i “LEO” /etc/passwd # not to be case sensitive

#serarch more than one files
grep -l "first" *.txt # 
grep -L "first: * .txt # not incluide first

#treat "bin" as one word (Exclude sbin)
grep `\<bin\>' /etc/password --color
grep -w 'bin' /etc/passwd

#multipile conditions
egrep '^root|bash$' passwd
```
