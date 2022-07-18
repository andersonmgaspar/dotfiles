# andi's dotfiles
:arrow_right: A simple repo for chezmoi dot files manager.

## Installation

:arrow_right: To **install** on new machines:
```bash
sh -c "$(curl -fsLS chezmoi.io/get)" -- init --apply andersonmgaspar
```

NOTE: if github asks for password change the remote link to **SSH**:
```
git remote set-url origin git@github.com:andersonmgaspar/dotfiles.git
```

:arrow_right: create chezmoi's source directory and a git repo on a new machine:
```bash
chezmoi init
```

## Usage
Daily commands [(source)](https://www.chezmoi.io/user-guide/command-overview/)

`chezmoi add $FILE` > adds $FILE from your home directory to the source directory.

`chezmoi edit $FILE` > opens your editor with the file in the source directory that corresponds to $FILE.

`chezmoi status` > gives a quick summary of what files would change if you ran chezmoi apply.

`chezmoi diff` > shows the changes that chezmoi apply would make to your home directory.

`chezmoi apply` > updates your dotfiles from the source directory.

`chezmoi edit --apply $FILE` > is like chezmoi edit $FILE but also runs chezmoi apply $FILE afterwards.

`chezmoi cd` > opens a subshell in the source directory.

