[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/jjmc89-bot/jjmc89-bot-toolforge/main.svg)](https://results.pre-commit.ci/latest/github/jjmc89-bot/jjmc89-bot-toolforge/main)

[JJMC89 bot](https://meta.wikimedia.org/wiki/User:JJMC89_bot), [JJMC89 bot II](https://meta.wikimedia.org/wiki/User:JJMC89_bot_II), [JJMC89 bot III](https://meta.wikimedia.org/wiki/User:JJMC89_bot_III), and [Magic links bot](https://meta.wikimedia.org/wiki/User:Magic_links_bot) run on [Wikimedia](https://www.wikimedia.org/) projects and are hosted on [Wikimedia Toolforge](https://toolforge.org/).

Toolforge setup and job management

## Clone and setup virtual environments
```shell
rm -fdr $HOME/repos && git clone --recurse-submodules --shallow-submodules https://github.com/jjmc89-bot/jjmc89-bot-toolforge $HOME/repos && toolforge-jobs run setup-venvs --command $HOME/repos/bin/setup-venvs --image python3.9 --wait
```

## Load jobs
```shell
toolforge-jobs load $HOME/repos/cronjobs.yaml
```
