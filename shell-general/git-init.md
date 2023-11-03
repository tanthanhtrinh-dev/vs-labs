
## [Ref fully document of Git](https://git-scm.com/docs)

### Git Init
```shell
git init; 
git add .; 
git commit -m 'Initial commit';
git remote add origin [repo_address];
git push --mirror --force;
```

### Git Init Option
```shell
# Clone the project, e.g. `myproject` is my project repository:
git clone https://github.com/tanthanhtrinh-dev/dotnet-tutorial.git

# Since all of the commits history are in the `.git` folder, we have to remove it:
cd dapr-labs

# And delete the `.git` folder:
git rm -rf .git

# Now, re-initialize the repository:
git init
git remote add origin https://github.com/tanthanhtrinh-dev/dotnet-tutorial.git
git remote -v

# Add all the files and commit the changes:
git add --all
git commit -am "Initial commit"

# Force push update to the main branch of our project repository:
git push -f origin main
```

```shell
git remote add mygit https://github.com/tanthanhtrinh-dev/dotnet-ref.git
git checkout mygit
git push --set-upstream mygit main
```