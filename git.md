Pages: [home](https://sm0rux.github.io/) - [git](https://sm0rux.github.io/git.html) - [anytone](https://sm0rux.github.io/anytone.html)

# Feel free to fork!

On this page I present how I use git and GitHub. I'm not a GitHub expert, not
even a programmer, but I will show the way I found out how to use git and
GitHub.

BR,

Pontus Falk ([sm0rux](https://github.com/sm0rux/))

---

Are you a git/GitHub newbie like I am? Feel free to fork this repo and
hopefully we can learn together. Why not start to add your name to the
[Contributors.md](https://github.com/sm0rux/sm0rux.github.io/blob/main/Contributors.md)
file?

## Copyright

Feel-free-to-fork

© Copyright 2019-2020 by Pontus Falk (sm0rux). All rights reserved.

This repository is publiced under Creative Commons Zero v1.0 Universal
license.

## How to contribute

### 1. Fork this repository

Click the "Fork" button in the upper right corner of this repository.

### 2. Clone your fork

Click the green "Clone or download" button and enter
```
git clone git@github.com:YourUserID/Feel-free-to-fork.git
```
in a terminal window on your computer. I prefer to collect all my repositories
in ~/GitHub, but this is of course up to you to decide.

In case you don't have a SSH key you can use
```
git clone https://github.com/YourUserID/Feel-free-to-fork.git
```

### 3. Make a link to the main repository

Now change directory to the repository and create a link to the main
repository. I suggest you call the link to the main repository `upstream`. You
add the link using the command
```
git remote add upstream https://github.com/sm0rux/feel-free-to-fork.git
```

As you normaly don't have the SSH key to the main repository, you can't use
the command `git remote add upstream
git@github.com:YourUserID/feel-free-to-fork.git` when adding `upstream`.

#### 3a. If your repository is the main repository

In case your repository is the main repository, then you don't have to create
the `upstream` link mentioned above.

### 4. Download the repository to your computer

First, got to the directory created in step 2, e.g.
```
cd ~/GitHub/feel-free-to-fork
```
and then pull the files using the command
```
git pull origin main
```

The main branch of my repository is `main` but this could be something else
for other branches. If the main branch is `source` then download the files
using the command
```
git pull origin source
```

### 5. Create a new branch

I suggest you create a new branch before starting to add or edit file(s).
Also, your new branch should be checked out. This is done using the command
```
git checkout -b NameOfYourNewBranch
```

Your new branch name could either just be a date, like `20190908` or a more descriptive name like `Added-My-Name-To-Contributors.md`.

### 6. Add or edit file(s)

Well - I leave up to what to do, but of course I recommend you to add your
name to the Contributors.md file :)

### 7. Add file(s) to the git index

This could be done either with the command
```
git add filename1.ext [filename2.ext]
```
or to add all files at once using the command
```
git add .
```

### 8. Make a commit

Now it's time to make a commit. Don't forget to mention what your commit will
do to the repository. This is done either with the command
```
git commit -m "Added my name to Contributors.md"  Contributors.md
[filename2.ext]
```
or, in case your commit require more than one file to be changed, more easily
with the command
```
git commit -a -m "Added my name to Contributors.md"
```

### 9. Push your contribution

Push your files. This is done with the command
```
git push origin NameOfYourBranch
```
where `NameOfYourBranch`is the name you used step 4.

### 10. Make a pull request

Now it's time to go back to the GitHub web site and make a pull request to get
your files incorporated in the main repository (in this repository).

## Make more contributions

Before making more contributions, be sure to have your fork up to date with
the main repository. This is done by giving the commands `git pull upstream
main` followed by the command `git push origin main`.

### In case your repository is the main repository

As mentioned in 3a above you don't have an upstream link if your repository is
the main repository. Instead you give the commands `git pull origin main` to
keep your local files up to date.

Then you can start the new contribution by following step 5-10 above.
