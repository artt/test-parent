## Instructions

### Preparation

1. Clone this repo.
2. `cd` into `/public`. This is supposed to be the folder created by a `build` script. In this step, the folder should be a child of the `test-parent` git repo.
3. Make changes to `test.txt`. Maybe just add one line so you can see the history is working.

### Doing stuff
1. We would like to make this another repo by itself. Do `git init`.
2. Suppose the deploy repo is at `test-child`. We do the following:

```
git remote add origin https://github.com/artt/test-child.git
git fetch
git reset origin/main
git commit -am "commit message here"
git push --set-upstream origin main
```

3. Check out the result [in this repo](https://github.com/artt/test-child/commits/main/test.txt)

That's it! 🎉
