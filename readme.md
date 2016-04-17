#.dotfiles


A collection of my `.dotfiles` from my OSX developer environment. Keeping things clean and organised, and basic profiling for a fresh OS Install.

## deprecated



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

---

## New Zsh setup using Prezto

1. install **Zsh** from [http://www.zsh.org/](http://www.zsh.org/)
2. run `zsh`
3. run `git clone --recursive https://github.com/sorin-ionescu/prezto.git "${ZDOTDIR:-$HOME}/.zprezto"`
4. run `setopt EXTENDED_GLOB
  for rcfile in "${ZDOTDIR:-$HOME}"/.zprezto/runcoms/^README.md(.N); do
    ln -s "$rcfile" "${ZDOTDIR:-$HOME}/.${rcfile:t}"
  done`
5. then `chsh -s /bin/zsh`
6. find `~/.zshrc` and open it and add the imports list from above (ie: the dotfiles)
7. download this [osx terminal themes](https://github.com/lysyi3m/osx-terminal-themes) repo, select one and double click the `*.terminal` to set it as your base terminal theme.
8. Change fonts/spacing as you like.
9. now locate `~/.zpreztorc` config file and add the following `'git' \
  'syntax-highlighting' \
  'history-substring-search' \` to the modules to load
10. find `syntax-highlighting` in current file, and unblock where to to highlight, same with `color output`
11. Customisation of the prezto theme is done by using `prompt -l` to list the available themes, and by using the `-s <name>` to save it.


###Done.
ps.to.self `.ssh-paths` is not included, because you are not stupid. Do a local transfer. 