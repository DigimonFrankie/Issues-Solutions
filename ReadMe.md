# 1. Issues & Solution

## 1.1. About
-- --  
This is a note for the issues I met and the solutions for them. The situtation includes issues in `python`, `GitHub`, `MySQL`, `Jupyter Lab` and other random stuff.

# 2. Table of Contents
-- --
- [1. Issues & Solution](#1-issues--solution)
  - [1.1. About](#11-about)
- [2. Table of Contents](#2-table-of-contents)
- [GitHub](#github)
  - [Push to new repo](#push-to-new-repo)
  - [Change repo url](#change-repo-url)
- [3. Jupyter Lab](#3-jupyter-lab)
  - [3.1. Autocomplete](#31-autocomplete)
  - [3.2. Ipython is Not defined](#32-ipython-is-not-defined)
- [4. Sklearn](#4-sklearn)
  - [4.1. metrics](#41-metrics)
    - [4.1.1. r2_score](#411-r2_score)



# GitHub

## Push to new repo
```
echo "# reponame" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin [repo_url].git
git push -u origin main
```

## Change repo url
Check current

```
git remote -v
```

Set new url
```
git remote set-url origin [repo_url].git
```

# 3. Jupyter Lab

## 3.1. Autocomplete  
When Autocomplete is disabled, use this code to activate the function.
```
%config Completer.use_jedi = False
```
- [Back to content](#2-table-of-contents)


## 3.2. Ipython is Not defined
**Option 1:**
```
%matplotlib inline
```
**Option 2:**
```
pip3 install ipympl
```
And then add %matplotlib ipympl before plot.

**Option 3:**


1. Jupyterlab supports `jpympl`.

2. You must put `%matplotlib widget` in the very beginning of the jupyterlab.

You can change to %matplotlib inline in specific cell, and active %matplotlib widget again if needed.

[Link](https://stackoverflow.com/questions/51922480/javascript-error-ipython-is-not-defined-in-jupyterlab) 
- [Back to content](#2-table-of-contents)




# 4. Sklearn

## 4.1. metrics

### 4.1.1. r2_score

The latest sklearn version:
```
from sklearn.metrics import r2_score
```

- [Back to content](#2-table-of-contents)