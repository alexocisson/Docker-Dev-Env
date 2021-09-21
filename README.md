# Docker Developper Environement

This git is an easy to deploy developper environement docker container with the help of Bash scripts.
At the moment, everything happens in the dev folder. A docker install script for ubuntu may be added at the root of the project later.

## Scripts

Go in the scripts folder with the terminal and use `./script-name` to use a script.

### Dev scripts:

- `build`		Build the docker image base under the name of **build/dev:base**
- `start`		Runs **build/dev:base** in a container and open a terminal. An argument can be passed which will be added after the **base** tag.
- `stop`		Stops all the running Docker containers
- `clean-docker`	`stop` then deletes all the **dev/** and <none> images for a rebuild
- `commit`		Commits the running container to a new image **build/dev:base-name-of-the-commit` where name-of-the-commit is the arg passed to the command
