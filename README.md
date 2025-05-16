# syfo-meta

The goal of this repoository is to provide quality-of-life tools for the developers of team-esyfo.

First and foremost, it provides a tool to fetch and update all the repositories the team manages with simple bulk commands.
This is done with the tool [meta from npm](syfomotebehov)

## Install

```bash
npm install -f meta
```

## https VS ssh

This tool uses https when spesifying the location of the git repositories.
If you prefer to us ssh, you can add configuration to your .gitconfig so it automatically rewrites them

```bash
git config --global url."git@github.com:".insteadOf "https://github.com/"
```

## Fetch all repositories

```bash
meta git update
```

## Pull updates from all repositories

```bash
meta git fetch
```
