# Packer completion

Bash completion for [Packer](http://www.packer.io).

* `packer b<tab> # => packer build`
* `packer f<tab> # => packer fix`
* `packer i<tab> # => packer inspect`
* `packer v<tab> # => packer validate`

Tabbing twice with no arguments will return a list of all available commands for completion.
```bash
packer <tab><tab>
# build fix inspect validate
```

## Requirements
* [Packer](http://www.packer.io/docs/installation.html)
* Bash
* Bash completion v1.3+ (running 1.1+ should work, but I haven't tested it)

## Installation
### Mac OS X
```bash
brew tap ipwnstuff/formulae
brew install packer-completion

# Then add the script into your .bashrc
if [ -f `brew --prefix`/etc/bash_completion.d/packer-completion.bash ]; then
    source `brew --prefix`/etc/bash_completion.d/packer-completion.bash
fi
```

### Other
```bash
wget https://raw.github.com/ipwnstuff/packer-completion/master/packer-completion.bash -P ~
echo "source ~/.packer-completion.bash" >> ~/.bashrc`
```
