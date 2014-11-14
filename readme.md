#.dotfiles
===

A collection of my `.dotfiles` from my OSX developer environment. Keeping things clean and organised, and basic profiling for a fresh OS Install.

##How to use

__Prerequisite__ make sure you have a `.bin/` with [init z!](https://github.com/rupa/z) placed there.

Clone this set into `~/.dotfiles/`, and then create a `.bash_profile` with the following:

```
# imports
. ~/.dotfiles/.path
. ~/.dotfiles/.alias
. ~/.dotfiles/.functions
. ~/.dotfiles/.bash_prompt

# init z! (https://github.com/rupa/z)
. ~/.bin/z.sh
```

#Done.
ps.to.self `.ssh-paths` is not included, because you are not stupid. Do a local transfer. 