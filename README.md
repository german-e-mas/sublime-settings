# Sublime Settings

Sublime settings for easy sync between computers. This is meant for personal use.

---

## First time Setup

- Install [Sublime Text 3](https://www.sublimetext.com/).
- Install [Package Control](https://packagecontrol.io/).
- Initialize the repository in your current user's settings folder.

```
cd ~/.config/sublime-text-3/Packages/User/
git init
git remote add origin git@github.com:german-e-mas/sublime-settings.git
git pull origin master
git commit -am "Add settings and packages"
git push
```

**Note:** Syncing `Packages/` and `Installed Packages/` folders is not necessary. Once Package Control is installed, only the `Packages/User/` folder is required. The next time Sublime Text is installed, the packages are going to be isntalled with their correct versions. More info on Syncing [here](https://packagecontrol.io/docs/syncing).

---

## Use the repository to get the settings.

On another computer, you need to do the following:

```
cd ~/.config/sublime-text-3/Packages/User/
git init
git remote add origin git@github.com:german-e-mas/sublime-settings.git
git pull origin master
git reset --hard origin/master
```

Be careful: Your local files are going to be overwritten by the files from the repository. If you don't want this, backup your settings or remove the `--hard` flag.

---

## List of installed packages

- [SideBarEnhancements](https://packagecontrol.io/packages/SideBarEnhancements)
- [A File Icon](https://packagecontrol.io/packages/A%20File%20Icon)
- [VCS Gutter](https://packagecontrol.io/packages/VCS%20Gutter)
- [Color Hightlighter](https://packagecontrol.io/packages/Color%20Highlighter)
- [Markdown Preview](https://packagecontrol.io/packages/Markdown%20Preview)
- [SublimeLinter](https://packagecontrol.io/packages/SublimeLinter)
- [Typescript](https://packagecontrol.io/packages/TypeScript)
- [Babel](https://packagecontrol.io/packages/Babel)
- [SCSS](https://packagecontrol.io/packages/SCSS)

---

## Source

- [Using Git to sync Sublime Text settings](https://medium.com/@devmount/using-git-to-sync-sublime-text-settings-f70b8dc7a40d) - By [Andreas Müller](https://medium.com/@devmount)
