# first-repo

## How to push code to github
1. create a github account, if you don't have any
1. open your project in any code editor
1. initialialize a local git repo `git init`
1. made changes to your code 
1. `git add .`
1. `git commit -m 'descriptive message about feature or code changes'`
1. now addyour reote repo
1. `git remote add origin remote-repo-url'`
1. `git push origin master`
1. now provide your username and password and you are good to go
1. see the updated code at github


## how to push code to github with SSH (no password needed)

1. get your ssh keys
1. `ssh-keygen -t rsa -b 4096 -C "my_email@example.com"`
1. press `enter` and provide required info
1. be sure to setup ssh your passphrase (and remember it). you will need it when you are connecting to github or any other ssh agent
1. now add generated ssh keys to ssh-agent
1. `eval "$(ssh-agent -s)"`
1. `ssh-add ~/.ssh/id_rsa`. replace `~/.ssh/id_rsa` with youe ssh key file location
1. now go to [github settings](https://github.com/settings/keys)
1. copy your ssh key in `.pub` file.
1. to copy ssh key type `code ~/.ssh/id_rsa.pub` if you have vs code and copy your keys
1. paste it at github ssh key and give it a suitable name
1. now taste your ssh with github
1. ssh -vT git@github.com
1. if it says successfully authenticated, then your setup is ok
1. sometimes it will ask for password when you push your code to github so provide your passphrase.
1. that's it

