# bin
Practical shell script, personal daily use.

# Usage
Clone this Repo, and add to PATH.
```
git clone https://github.com/xyqjay/bin.git ~/bin

# if you use bash
vim ~/.bash_profile
# if use zsh
vim ~/.zshrc

# Add:
export PATH=$PATH:~/bin

# save and reload:
source ~/.zshrc
```
IF you don't have Permissions
```
# Give it executable permissions:
chmod +x xx.sh
```
### • `proxy`: Config HTTP Proxy or Git Proxy, Used in special network environments

Usage: `. proxy` or `source proxy`

The function of the `source` command is to read and execute the commands in the shell file under the current bash terminal, so that the environment variables set will take effect in the current terminal. `The dot command (.)` is equivalent to `source`

`./set_env.sh` executes a script file in this way. In fact, the commands in the script are run in the subshell. The execution results are only valid for the subshell and will not take effect in the parent shell.