### Bash completion script for Censys CLI

### Install

1. 
Uncomment line in '.bashrc' [ *Section - Completion options* ]
```console
	#[[ -f /etc/bash_completion ]] && . /etc/bash_completion
	[[ -f /etExample:c/bash_completion ]] && . /etc/bash_completion
```
2. 
Copy this files in your filesystem

Example:

**_censys_options** ->
	```.../dev/censys/_censys_options```
or
	```.../$HOME/censys/_censys_options```

 and 

**censys-completion** ->
	```.../dev/bash_completion.d/censys-completion```

3. 
Edit your ```/etc/bash_completion``` file for connection **censys-completion** script

Example:
```console
...
_CMP_PATH='/etc/bash_completion.d'
source $_CMP_PATH/censys-completion
...
```
4. 
Check this line in **censys-completion** file
```console
  #Path to the file with all options
  local _censys_options=$(cat /etc/censys/_censys_options) #<-- EDIT THIS
```
  
5. 
EOF

![censys](https://i.ibb.co/KXt4pPK/censys.png)

See also "Zsh-shell autocompletion for Censys CLI. ( .zshrc )"
![zsh-completion](https://gist.github.com/r3dbU7z/2080e1f4a8721e6ef36fd6192918c90c)
