### bash commands:

```
ls
pwd
which bash
cd / && ls  # root directories
mkdir
ll  ## long list
cd ./
cd ..
touch <file>

sudo su  # super user (root access)

echo "test string" >> <file>
cat <file>

mkdir <dir>
cp <source_path> <destination_path>
mv <source_path> <destination_path>
rm <source_path>
rm -r <directory>
```

permission blocks \[3], owner, group, user
d ➡ directory
r ➡ read
w ➡ write
x ➡ execute
`(d)(rwx)(r-x)(r-x)`
`-x` ➡ no execute
`chmod +x <file>` ➡ make file executable

### Linux packages:

```
sudo apt-get update

sudo apt-get upgrade

sudo apt install <package>

which git   # path to the package, git example
```

### Shell script:

```
chmod +x <path_to_file>  # add executable permission
```

### Git:

```
git revert <commit_hash>  # rollback to previous commit

git reflog  # shows all action to in the git directory

git reset --hard <commit_hash>

git switch -c feature/<feature_name>  # checkout alternative

git rebase # avoid an additional merge commit
```

Head: pointer to working branch

#### Braching workflow:

- dev: merge feature branches
- stage: testing before going live
- main: always live (in production)

#### SSH

```
shh-keygen -t ed25519 -C "example@email.com"
```

Git Games: `Oh my Git`, `learngitbranching.js.org`