# Shell 🐚

Settings for my dev environment.

## Setup

### Install everything
1. Get [iTerm2](https://www.iterm2.com/) as a terminal replacement.
2. Within iTerm download [oh my zsh](https://ohmyz.sh/).
3. Next, install [pure-prompt](https://github.com/sindresorhus/pure). Use the homebrew installation.
4. Get [iterm2-snazzy](https://github.com/sindresorhus/iterm2-snazzy).
5. Also get [zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting).

### iTerm customization
Here are a couple settings I like to get a full clean version of iTerm where it looks very similar to my old Hyper setup.
1. Use Minimal Theme
2. Change font to Menlo
3. Use a custom window title and set to `~`
4. In the "Panes" section uder "Appearance", set margins for Top/Bottom and Left/Right (Side) to 15

### Final touch ups
1. If you want to remove the "last login" text at the start of each session do:
```
touch .hushlogin
```
2. If the "you've got mail" message also pops up, check out [this](https://apple.stackexchange.com/questions/28745/how-do-i-delete-all-terminal-mail) thread to delete that message.

### Symlinks
You'll want to create symlinks between the config files and files in this repo.

Remove the original config file:
```
rm ~/.zshrc
```

Next, create the symlink
```
ln -s ~/path/to/this/repo/.zshrc ~/.zshrc
```

Now, any changes that happen in this repo will be applied when pulled down.
