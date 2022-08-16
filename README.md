![GitHub package.json version (subfolder of monorepo)](https://img.shields.io/github/package-json/v/rynodivino/git-actions-standard-version)

# github-actions-standard-version

## Description
The purpose of this repo is to provide a simple example of how to use github actions, with standard-version and conventional commits, to automate versioning and changelog generation.  Whenever code is merged (or pushed) to the branch specified in the release.yml file - a new git workflow will kick off, and automatically.

## Before Getting Started
If you're here, it's assumed you're familiar with [standard version](https://github.com/conventional-changelog/standard-version), [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/), etc...  - but if you're not you should browse through the resources at the bottom of this README to understand how those work.

## Getting Started
 * Simply add the following directory and file as seen in this repo ```.github/workflows/release.yml```.
 * Run the first release locally - see [first release](https://github.com/conventional-changelog/standard-version#first-release), and push the tag ```git push --follow-tags origin main```
 * After the manual first release, any new prs merged into main (or whatever branch you chose) should be set to pop (automated)


## Optional
 * You can rename the yaml file to whatever you like
 * Work off a different branch (I used _main_ for this demo)
 * Move the npx and git push tags logic to package.json scripts
 * Remove the [.versionrc](https://github.com/conventional-changelog/standard-version#configuration), and just use the defaults
 * Add pre-commit hooks to ensure commit messages adhere to the correct syntax
 * Party

## Resources
* [standard version](https://github.com/conventional-changelog/standard-version)
* [semver.org](https://semver.org/)
* [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/)
* [github actions](https://github.com/features/actions)
