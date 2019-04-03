# Sublime Text Settings

This repository contains my personal settings for [Sublime Text 3](https://www.sublimetext.com/). It allows me to easily synchronize my settings in different computers.

---

## First steps

Install Sublime Text and Package Control, if you haven't already.

- Install [Sublime Text 3](https://www.sublimetext.com/).
- Install [Package Control](https://packagecontrol.io/).

I use the font FiraCode. You need to install it as well.

```
sudo apt-get install fonts-firacode
```

---

## Push your settings to this repository

- Initialize the repository in your current user's settings folder.

```
cd ~/.config/sublime-text-3/Packages/User/
git init
git remote add origin git@github.com:german-e-mas/sublime-settings.git
git pull origin master
git commit -am "Add settings and packages"
git push
```

**Note:** Syncing `Packages/` and `Installed Packages/` folders is not necessary. Once Package Control is installed, only the `Packages/User/` folder is required. The next time Sublime Text is installed, the packages are going to be installed with their correct versions. More info on Syncing [here](https://packagecontrol.io/docs/syncing).

---

## Pull your settings from this repository

- Whenever you want to pull the settings, you need to do the following:

```
cd ~/.config/sublime-text-3/Packages/User/
git init
git remote add origin git@github.com:german-e-mas/sublime-settings.git
git pull origin master
git reset --hard origin/master
```

**Be careful:** Your local files are going to be overwritten by the files from the repository. If you don't want this, backup your settings or remove the `--hard` flag.

---

## Source

- [Using Git to sync Sublime Text settings](https://medium.com/@devmount/using-git-to-sync-sublime-text-settings-f70b8dc7a40d) - By [Andreas Müller](https://medium.com/@devmount)
