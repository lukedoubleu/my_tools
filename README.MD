## create_remote_repo
### Creates remote repository on github.com, from the command line, with repo name as the argument, clones that newly created repo with a README.md in your current working directory, appends a line to the README.md, then commits and pushes the README.md back to remote, on main or master branch.
      ./create_remote_repo REPONAME

#### You will need to have a personal access token (PAT) that allows repo creation
#### You will need to set two environment variables:
     export GIT_TOKEN=YOUR_PAT
     export GIT_USER=YOUR_GITHUB_USERNAME

#### In order to prevent creation of the new git repo in this [my_tools] git's directory on you local machine (i.e. running `./create_remote_repo REPONAME` will create the git repo REPONAME in this `my_tools` local git directory, probably not what you want). Ergo, add this (my_tools) directory to your PATH variable, so you can run <b>create_remote_repo</b> in any directory on your local machine.

E.g. Once you added to PATH, you can run <b>create_remote_repo REPONAME </b> in ~/here/orthere/anywhere to create local repo ~/here/orthere/anywhere/REPONAME/
      ./delete_remote_repo REPONAME (or, `just delete_remote_repo REPONAME` if you added this git to your PATH variable) will delete remote REPONAME
