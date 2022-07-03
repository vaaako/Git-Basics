# Git Basics

#  Genarate SSH KEY
> You just need to do this one time

## Generate ssh-key
- `ssh-keygen -t rsa -C "email@gmail.com"` (**Hit ENTER 3 times**)

## Add Key
- `ssh-add ~/.ssh/id_rsa`

- If you get an error: `ssh-agent -s`
- If you get an error again: `eval ssh-agent -s`

## Add Public Key
- `cat ~/.ssh/id_rsa.pub` (copy)

- Go to <a href="https://github.com" target="_blank">Github</a>
	- Settings > SSH and GPG keys > New SSH Key > *PASTE YOUR KEY* > Add SSH key



# CREATING A PROJECT
## CREATE .gitignore
- Create a file named *.gitignore*
- Write all the files you don't want to git add on github

```.gitignore
.env
package-lock.json
node_modules/
```

## Add files to the project
- `git init`
- `git add .`  (Add all files)
	- `git add [file1, file2...]` (Add individual files)
- `git commit -m "first commit"` (Always need to make a commit)
- `git branch -M main` (Create branch)
- `git remote add origin git@github.com:vaaako/REPOSITORY'S-NAME.git` (Add repository)
- `git push -u origin main` (Apply changes)
