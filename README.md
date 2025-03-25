# git-switchto

Git utility command to automatically do stash/unstash when checking out branches withtin the same workdir.

## Installation

Download `git-switchto` file and put into `~/.local/bin/git-switchto` (should be added to `$PATH`) or any other diretory in the `PATH`.

## Usage

```sh
git branch # on dev

# do some changes to the files...

git checkout main
# will result in possible error
# "... Please, commit your changes or stash them before you can merge."

git switchto main
# will automatically stash everyting in stash with name `branch:dev` and later unstash it

git branch # on main
```
