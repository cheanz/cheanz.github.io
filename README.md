
# SHELL wissen
# branch -c
Ich habe einen Unterschied zwischen 2 Befehlen gefunden.
I found a difference between 2 commands.
```
bash -c "echo $0 is $0, $1 is $1, $2 is $2" foo bar biz
bash -c 'echo $0 is $0, $1 is $1, $2 is $2' foo bar biz
```
`man bash'  
information uber 
![image](https://user-images.githubusercontent.com/59786755/182548955-229f35e8-300a-4322-8fb8-066f1275f6a1.png)

# single quote VS double quotes
 it’s important to emphasize that the script argument (the command string after -c) must be enclosed with single quotes and not double quotes.  Otherwise the parent shell (in which you type the above command lines) would resolve any positional parameters in the script argument in the context of the parent shell
" ":current shell will expand $0 and so forth excactly replace it with /bin/bash/  
'': current shell will not expand $0 in it until all the parameters are taken into account.  --zhang yt
