# **Interactive Rebase :**

It is a tool for opitmizing and cleaning our commit history.

**Use cases :**
* change a commits message.  
* delete commits.
* reorder commits.
* combine multiple commits into one and vice-versa.
* reopen commits.

>NOTE:  
    Do **NOT** use it on commits already pushed to Github.

Use it for cleaning up commit history before merging it to a team branch.  


>NOTE:  
    If we want to make changes to the most recent commit, we could use   
    ```
    git commit --amend -m "an updated commit message"
    ```
___  

### **Steps for interactive rebase :**

1. Determine our base commit / how back we wanna rewind.

```
git rebase -i HEAD~3
```  

2. An editor window / Gitlens tool pops up.  
3. Choose the operation to be performed on the commit.

```
# Commands:
# p, pick = use commit
# r, reword = use commit, but edit the commit message
# e, edit = use commit, but stop for amending
# s, squash = use commit, but meld into previous commit
# f, fixup = like "squash", but discard this commit's log message
# x, exec = run command (the rest of the line) using shell
# d, drop = remove commit
```

4. Make the changes to the second window opening up.
5. Save and close.
6. Check if the changes took place.
___
