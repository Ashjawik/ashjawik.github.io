# git usage <!-- omit in toc -->

- [Start with the master branch](#start-with-the-master-branch)
- [Create a feature branch](#create-a-feature-branch)
- [Update, add, commit, and push changes](#update-add-commit-and-push-changes)
- [Push feature branch to remote](#push-feature-branch-to-remote)
- [Pull request](#pull-request)

This project uses the [feature branch workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/feature-branch-workflow)

Each feature development takes place in a seperate branch called feature-branch.
Feature branch should always be realted to a feature and only contain those changes.
For all new posts or changes on documentation the branch `develop` is used

## Start with the master branch

All feature branches are created off the latest code state of a project aka master branch.

```cmd
git checkout master &&
git fetch origin &&
git reset --hard origin/master
```

## Create a feature branch

if you create a new feature branch that wasn't there before:

```cmd
git checkout -b new-feature
```

otherwise use the following command to reset the existing branch to latest master

```cmd
git checkout your-existing-branch &&
git reset --hard master
```

## Update, add, commit, and push changes

If your feature-branch is not rebased to current master:

```cmd
git pull --rebase origin master
```

otherwise continue with

```cmd
git status
git add <some-file>
git commit
```

## Push feature branch to remote

```cmd
git push -u origin new-feature
```

## Pull request

Create a pull request through github UI
