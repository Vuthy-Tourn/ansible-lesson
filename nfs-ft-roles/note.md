## Note
***
### Working with git modules 
               
```bash 

# Removes the nfs directory ONLY from Git’s tracking, but keeps the files on disk.
git rm --cached -r nfs-ft-roles/roles/nfs

# Adds the repository as a Git submodule at the given path.
git submodule add --force https://github.com/Vuthy-Tourn/ansible-nfs-role.git nfs-ft-roles/roles/nfs

```

### Working with Ansible Galaxy 
```bash 

ansible-galaxy install git+https://github.com/Vuthy-Tourn/ansible-nfs-role.git,main 

ansible-galaxy install git+https://github.com/Vuthy-Tourn/ansible-nfs-role.git,main --roles-path .

```