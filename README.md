# shell

A collection of functions and aliases

## usage

```
$ git clone https://github.com/radavis/shell
$ cp shell/config/.vars ~/.vars
```

Add the following to your runtime config file.

```
# ~/.bashrc, ~/.zshrc, ~/.whateverrc

# load vars
if [[ -a ~/.vars ]]; then
  source ~/.vars
fi

# load aliases
for file in $PROJECTS/shell/aliases/*; do
  source $file
done

# load functions
for file in $PROJECTS/shell/functions/*; do
  source $file
done
```
