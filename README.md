# Git course

Exercises made on the [open git course](https://fitech.io/fi/opinnot/git-open/) organized by university of Tampere.

## Exercise 1: Initializing a repository

Commands used:
```git
git clone https://github.com/teijatestaaja/open-git-course.git
cd open-git-course
git add .
git commit -m "added hello world"
git push
```

## Exercise 2: File version return

Commands used:
```git
git remote add matskut https://course-gitlab.tuni.fi/git-course/basics-materials.git
git fetch matskut
git merge matskut/master --allow-unrelated-histories
git log
git checkout dd8c56cede9b109c1df7bda13abc1b1b7b79ed0b
git checkout –b temp #makes a new branch from current detached HEAD
git branch –f master temp #update master to point to the new <temp> branch
git merge origin/master --allow-unrelated-histories
git push
```

## Exercise 3: Branching

Commands used:
```git
git remote add keskitaso https://course-gitlab.tuni.fi/git-course/intermediate-branches.git
git fetch keskitaso
git merge keskitaso/master --allow-unrelated-histories
git checkout -b feature/create-awesome
git add .
git commit -m "added new feature"
git push --set-upstream origin feature/create-awesome
git checkout -b release
git add .
git commit -m "added new release"
git push --set-upstream origin release
```

## Exercise 4: Normal merge

Commands used:
```git
git remote add normaalimerge https://course-gitlab.tuni.fi/git-course/intermediate-normal-merge.git
git fetch normaalimerge
git merge normaalimerge/master --allow-unrelated-histories
```