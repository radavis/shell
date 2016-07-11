# shell

A collection of functions and aliases

# usage

```
$ git clone http://github.com/radavis/shell
```

Add the following to your runtime config file.

```
# ~/.bashrc, ~/.zshrc, ~/.whateverrc

# place environment variables in ~/.vars
if [[ -a ~/.vars ]]; then
  source ~/.vars
fi

for file in /Users/rd/code/shell/aliases/*; do source $file; done
for file in /Users/rd/code/shell/functions/*; do source $file; done
```