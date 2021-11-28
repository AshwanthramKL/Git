# **Submodules :**  

* It is a git repo nested inside a parent repo.  

* It enables a Git repository  to incorporate and track version history of external code ( 3rd party code ).

* Contents of a submodule are not stored in the parent repo.

* Parent repo only stores the remote URL, the local path inside the main project and checked out revision.
___

## **Creating a submodule folder :**

**STEP 1 :** Create folder to store submodule.  
**STEP 2 :** Use the following command.
```
git submodule add [ssh link]
```
**STEP 3 :** [Commit the changes.](https://github.com/AshwanthramKL/Git/blob/main/1.%20Git%20Commands.md#commit-) 

___

### **Cloning a repo which contains a submodule :**  

The submodules won't be available initially.   
To access those perform the following command after stepping into the submodules folder.

```
git submodule update --init --recursive
```  

**[ OR ]**

To avoid the extra command use this.

```
git clone --recursive-submodules [ssh link]
```

___
