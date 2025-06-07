# Git Foo

## 1- Where am I? Am I clean?

```bash
git status
```
## 2- What does my commit history look like?

```bash
git log
git log --oneline --graph --all --decorate
```

## 3- How can I alias a long Git command?

```bash
git config --global alias.lg "log --oneline --graph --all --decorate"
```

## 4- What have I changed since my last commit?

```bash
git diff HEAD
```

## 5- I messed up! How can discard ALL changes since my last commit?

```bash
git reset --hard
```

## 6- How do I switch between EXISTING branches?

```bash
git checkout somebranch
```

## 7- How do I create a NEW branch off of my current branch and move to it?

```bash
git checkout -b thenewbranch
```

## 8- How do I cut & paste changes across branches?

```bash
git stash
# check out the other branch...
git stash pop
```

## 9- How do I MERGE a branch into another?

```bash
git checkout main       # if I want to merge commits into main
git merge featurebranch # merges featurebranch commits into main
```

## 10- How do I update my local branch with commits from GitHub?

```bash
git fetch             # makes local aware of changes in remote
git checkout main     # in this example we wish to update main
git merge origin/main # merges main from GitHub into local main
```
