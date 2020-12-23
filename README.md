# git-templates


## Features

- [x] Copies hooks into `.git/hooks` on `git clone` and `git init` given the
      install settings in this README

### ActivityWatch (aw)

- [x] Send events to bucket `aw-git-hooks_$HOSTNAME` on post-commit or post-checkout
- [x] Add unique list of issues to the aw event
- [x] Support Jira issues, e.g., `MYPROJECT-123`
- [x] Support GitHub/GitLab issues, e.g., `#123`
- [x] Use commit timestamp for post-commit event
- [x] Check effect wenn using duration (e.g., 1h) in event. Needs duration > 0
      to be visible in timeline -> 2s. If set to 1h and another event is sent to
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

As soon as a new repo is cloned or initialized the hooks are copied to the repo's `.git/hooks` folder.

