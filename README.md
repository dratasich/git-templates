# git-templates


## Features

- [ ] Check git clone and git init copies the hooks

### ActivityWatch

- [x] Send events to bucket `aw-git-hooks_$HOSTNAME` on post-commit or post-checkout
- [x] Support Jira issues, e.g., `MYPROJECT-123`
- [ ] Support GitHub/GitLab issues, e.g., `#123`
- [ ] Use commit timestamp for event
- [ ] Check effect wenn using duration (e.g., 6h) in event
- [ ] Add branch
- [ ] Add first line commit message (summary)


## Install

```bash
$ cd ~
$ git clone git@github.com:dratasich/git-templates.git .git-templates
$ git config --global init.templatedir '~/.git-templates'
```

As soon as a new repo is cloned or `git init` the hooks are copied to the repo's `.git/hooks` folder.

