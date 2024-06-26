# Contributing

## Images
Within `objects/images` 

Images should be as small in size as possible. (Preferably under 500kb)

__Images are structures as:__

`object_namex1.png` for the first image (Image first slot)

`onject_namgex2.png` for the second image (Image second slot)

## Request for changes/ Pull Requests
You first need to create a fork this repository to commit your changes to it. Methods to fork a repository can be found in the [GitHub Documentation](https://docs.github.com/en/get-started/quickstart/fork-a-repo).

Then add your fork as a local project:

```sh
# Using HTTPS
git clone https://github.com/BryceCanyonCounty/redbackup.git

# Using SSH
git clone git@github.com:BryceCanyonCounty/redbackup.git
```

> [Which remote URL should be used ?](https://docs.github.com/en/get-started/getting-started-with-git/about-remote-repositories)

Then, go to your local folder

```sh
cd redbackup
```

Add git remote controls :

```sh
# Using HTTPS
git remote add fork https://github.com/YOUR-USERNAME/redbackup.git
git remote add upstream https://github.com/stevemao/redbackup.git


# Using SSH
git remote add fork git@github.com:YOUR-USERNAME/redbackup.git
git remote add upstream git@github.com/stevemao/redbackup.git
```

You can now verify that you have your two git remotes:

```sh
git remote -v
```

## Receive remote updates
In view of staying up to date with the central repository :

```sh
git pull upstream master
```

## Choose a base branch
Before starting development, you need to know which branch to base your modifications/additions on. When in doubt, use main.

| Type of change                |           | Branches              |
| :------------------           |:---------:| ---------------------:|
| Documentation                 |           | `development`              |
| Bug fixes                     |           | `development`              |
| New features                  |           | `development`              |
| New issues models             |           | `YOUR-USERNAME:patch` |

```sh
# Switch to the desired branch
git switch master

# Pull down any upstream changes
git pull

# Create a new branch to work on
git switch --create patch/1234-name-issue
```

Commit your changes, then push the branch to your fork with `git push -u fork` and open a pull request on [the Github-issue-templates repository](https://github.com/stevemao/github-issue-templates/) following the template provided.
