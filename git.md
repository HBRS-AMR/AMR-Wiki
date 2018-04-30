# Using Git to work on your repository

## 1. Configuring your upstream

To set up the master repository at https://github.com/HBRS-AMR/AMR-SS18 as your upstream, go to the local clone of your repository, open a terminal and type the following:
```
git remote add AMR-SS18 https://github.com/HBRS-AMR/AMR-SS18
```
Make sure to pull from this upstream regularly to get the code for the new assignments:
```
git pull AMR-SS18 master
```

New assignments will always be uploaded to the AMR-SS18 repository. To get the code for the assigments you have to pull from this repository as explained above.

## 2. Git workflow

When working with Git please make sure to always use the following steps:

### 2.1 Pull from *your* repository

You are not the only one working on your repository. I will upload grades to your repository and later on other team members will also work on the same repository.

Therefor please make sure that you pull from your repository before pushing anything and especially before pulling from the **AMR-SS18** repository.
If you don't do this you might overwrite any changes that are in your remote repository (e.g. the one on GitHub).

Please execute the following command:

```
git pull origin master
```

### 2.2 Pull from the AMR-SS18 repository

This only needs to be done after the lab class when the new assignment has been uploaded.

For this you execute the command described in section 1.

```
git pull AMR-SS18 master
```

### 2.3 Push to *your* repository

Your code should always be uploaded to *your* repository. Please make sure to pull before pushing to make sure you have all remote changes in your repository.
For this you want to execute:

```
git pull origin master
git push origin master
```

If you work on a different branch please change master to the name of your branch.

### 2.4 *Never* do a force push

A force push as executed by the following command

```
git push --force origin master
```

or 

```
git push -f origin master
```

should **never** be done. This will ignore the state of your remote repository and just overwrite it with your local copy. The history of your repository will be overwritten and if you are working in a team there is a good chance you delete the work of other team members.

If you work in a company there is a good chance this will get you fired.
 
