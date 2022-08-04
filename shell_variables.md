# $@ vs $*
$@ keeps spacess
while $* doesn't

# shift
# $$
`echo $$`   
to get the current process id. 
You can also alternate them with
```
ps -aux
```
to get all the processes' ids.
# $!
 PID of the last run background process.
# IFS
It means internal field seperator.
default value is SPACE TAB NEWLINE
