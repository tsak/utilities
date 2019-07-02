# set-github-credentials

A script to set the git username and email in the current folder to
values stored in `~/.github-credentials`

## Install

Put it somewhere in your path, for example `$HOME/.local/bin`

```bash
PATH="$HOME/.local/bin:$PATH"
```

Created `$HOME/.github-credentials` with

```
GITHUB_EMAIL=bar@baz.com
GITHUB_USERNAME=foo
```

## Run

```bash
mkdir foo && cd foo
git init
set-github-credentials
```

### Output

```
Git user.email was set to 'bar@baz.com'
Git user.name was set to 'foo'
```
