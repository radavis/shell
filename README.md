# shell

A collection of functions and aliases

## usage

```
$ git clone https://github.com/radavis/shell
$ cp shell/.vars ~/.vars
```

Add the following to your runtime config file.

```
# ~/.bashrc, ~/.zshrc, ~/.whateverrc

# load vars
if [[ -a ~/.vars ]]; then
  source ~/.vars
fi

# load shell settings
for file in $PROJECTS/shell/{aliases,config,functions}/*; do
  source $file
done
```
