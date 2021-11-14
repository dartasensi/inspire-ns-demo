# vg-docker-template

This project uses a Vagrant configuration (see git repository `vg-docker`) as submodule to prepare the system. Refer to the main README of that module for further details.

_NOTE:_ to create this repository and add a git submodule, the following is a list of commands example

```bash
echo "# my repository" >> README.md
git init
git submodule add https://github.com/dartasensi/vg-docker.git
# editing files..
git add .
git commit -m "First revision"
# rename current branch to "main", to reflect GH default naming
git branch -M main
git remote add origin <http-to-your-repository>.git
git push -u origin main
```

## Execution

Execute `$ vagrant up` to initialize (and provision only the first time) the Ubuntu VM with Docker

## Tips

