# git-templates


## Features

- [ ] Check git clone and git init copies the hooks

### ActivityWatch (aw)

- [x] Send events to bucket `aw-git-hooks_$HOSTNAME` on post-commit or post-checkout
- [x] Add unique list of issues to the aw event
- [x] Support Jira issues, e.g., `MYPROJECT-123`
- [x] Support GitHub/GitLab issues, e.g., `#123`
- [x] Use commit timestamp for post-commit event
- [x] Check effect wenn using duration (e.g., 6h) in event, needs duration > 0
      to be visible in timeline -> 1s. If set to 1h and another event is sent to
      the bucket within the same hour, the events are overlapping, i.e., a new
      event does not stop the previous one.
- [x] Add branch
- [x] Add first line of commit message (summary/title)


## Install

```bash
$ cd ~
$ git clone git@github.com:dratasich/git-templates.git .git-templates
$ git config --global init.templatedir '~/.git-templates'
```

As soon as a new repo is cloned or `git init` the hooks are copied to the repo's `.git/hooks` folder.

