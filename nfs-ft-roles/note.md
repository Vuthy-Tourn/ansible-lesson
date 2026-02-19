## Note
***
### Working with git modules 
               
```bash 

# Remove from disk
rm -rf nfs-ft-roles/roles/nfs

# Adds the repository as a Git submodule at the given path.
git submodule add https://github.com/Vuthy-Tourn/ansible-nfs-role.git nfs-ft-roles/roles/nfs

```

### Working with Ansible Galaxy 
```bash 

ansible-galaxy install git+https://github.com/Vuthy-Tourn/ansible-nfs-role.git,main 

ansible-galaxy install git+https://github.com/Vuthy-Tourn/ansible-nfs-role.git,main --roles-path .

```