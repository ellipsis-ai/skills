# Ellipsis Skills
Skills published and available to install for the [Ellipsis bot](https://www.ellipsis.ai/)

## Development

### Initial setup
This repository uses Git submodules to link to individual skill repositories. After checking out the repo the first time:

1. Run `git submodule init` to setup the submodules.
1. Run `git submodule update` to checkout the current version of each skill.

### Create a pull request to sync remote versions
To update an individual skill to the latest master on that repository, e.g. the Lunch skill:

1. `git pull origin master` to sync your repo.
1. `git submodule update` to ensure you’ve checked out the current versions of each skill.
1. `git checkout -b update_lunch` to make a new branch for this change
1. `cd lunch` to move into the skill directory.
1. `git pull origin master` to grab the latest master from the remote skill repository
1. `cd ..`
1. `git commit -a -m "Synced to latest version of Lunch skill"`
1. `git push origin update_lunch`
1. Create a pull request on GitHub
