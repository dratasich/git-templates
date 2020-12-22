# git-templates

## Install

```bash
$ cd ~
$ git clone git@github.com:dratasich/git-templates.git .git-templates
$ git config --global init.templatedir '~/.git-templates'
```

As soon as a new repo is cloned or `git init` the hooks are copied to the repo's `.git/hooks` folder.

## TODO

[] Use commit timestamp for event
[] Check effect wenn using duration (e.g., 6h) in event
[] Add first line commit message (summary)
[] Delete old buckets
[] Check git clone and git init copies the hooks
