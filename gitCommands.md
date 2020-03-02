To Loose all work and get New
==============================

* git stash
* git pull


To Reset to the Head Revision
=============================

* git fetch origin
* git reset --hard origin/master
* git pull

 
To revert a bunch of bad commits
================================

# set local to the top to start revert from here onwards, one by one
git reset --hard ba33de70 
git clean -f -d
git pull 
#to revert a merge (++++ ONLY USE IF THERE IS A MERGE)
git revert -m 1 HEAD  
# to revert A regular conflict commit
git revert d80bcc6f 
git pull
git push
