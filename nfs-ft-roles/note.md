## Note
***
### Working with git modules 
               
```bash 
# Removes the nfs directory from Git tracking AND deletes it from the working directory.
git rm -r ansible-related/nfs-ft-roles/roles/nfs

# Restores folder back on disk if it was removed by git rm
git restore nfs

# Removes the nfs directory ONLY from Git’s tracking, but keeps the files on disk.
git rm --cached -r ansible-related/nfs-ft-roles/roles/nfs

# Adds the repository as a Git submodule at the given path.
git submodule add --force https://github.com/Vuthy-Tourn/ansible-nfs-role.git ansible-related/nfs-ft-roles/roles/nfs

```

### Working with Ansible Galaxy 
```bash 
ansible-galaxy install git+https://github.com/Vuthy-Tourn/ansible-nfs-role.git,main 

ansible-galaxy install git+https://github.com/Vuthy-Tourn/ansible-nfs-role.git,main --roles-path .

```