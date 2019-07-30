# Shell 🐚

Settings for my dev environment.

## Setup

### Install everything
1. Get (Hyper)[https://hyper.is/] as a terminal replacement.
2. Within Hyper download (oh my zsh)[https://ohmyz.sh/].
3. Next, install (pure-prompt)[https://github.com/sindresorhus/pure].
4. Get (hyper-snazzy)[https://github.com/sindresorhus/hyper-snazzy].
5. To have new tab in Hyper open up the same directory: (hypercwd)[https://github.com/hharnisc/hypercwd].
6. Also get (zsh-syntax-highlighting)[https://github.com/zsh-users/zsh-syntax-highlighting].

### Symlinks
You'll want to create symlinks between the config files and files in this repo. Make sure to do these commands in Terminal rather than Hyper as removing `.hyper.js` will cause Hyper to freak out and re-generate it.

Remove these two original config files:
```
rm ~/.zshrc
rm ~/.hyper.js
```

Next, create the symlinks
```
ln -s ~/path/to/this/repo/.zshrc ~/.zshrc
ln -s ~/path/to/this/repo/.hyper.js ~/.hyper.js
```

Now, any changes that happen in this repo will be applied when pulled down.
