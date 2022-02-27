# ZSH Docker Aliases

Defines [Docker][1] aliases and functions.

## How to Install

### With [zplug][2]

```sh
zplug "akarzim/zsh-docker-aliases"
```

### With [Oh My Zsh](https://ohmyz.sh/):
```sh
git clone https://github.com/akarzim/zsh-docker-aliases.git  ~/.oh-my-zsh/custom/plugins/zsh-docker-aliases
# then add `zsh-docker-aliases` to `plugins` in your .zshrc
```

### With [zinit][4]
```sh
zinit light akarzim/zsh-docker-aliases
```

## Aliases

### Docker

- `dk` is short for `docker`
- `dka` Attach to a running container
- `dka!` Attach to a running container by name
- `dkb` Build an image from a Dockerfile
- `dkd` Inspect changes on a container's filesystem
- `dkdf` Show docker filesystem usage
- `dke` Run a command in a running container
- `dkE` Run an interactive command in a running container
- `dkE!` Run an interactive command in a running container by name
- `dkh` Show the history of an image
- `dki` List images
- `dkin` Return low-level information on a container, image or task
- `dkk` Kill a running container
- `dkkh` Send `kill -s HUP` signal to a running container
- `dkl` Fetch the logs of a container
- `dkL` Fetch and follow (`-f`) the logs of a container
- `dkli` Log in to a Docker registry
- `dklo` Log out from a Docker registry
- `dkls` is alias for `dkps`
- `dkp` Pause all processes within one or more containers<Paste>
- `dkP` Unpause all processes within one or more containers
- `dkpl` Pull an image or a repository from a registry
- `dkplI` Pull all tagged images
- `dkph` Push an image or a repository to a registry
- `dkps` List containers
- `dkps!` Display the first matching docker container ID by name
- `dkpsa` List all containers (default lists just running)
- `dkr` Run a command in a new container
- `dkR` Run an interactive command in a new container and automatically remove the container when it exits
- `dkRe` like `dkR` and set entry point to `/bin/bash`
- `dkrm` Remove one or more containers
- `dkrmi` Remove one or more images
- `dkrmC` Clean up exited containers
- `dkrmI` Clean up dangling images
- `dkrmV` Clean up unused volumes ( Docker >= 1.9 )
- `dkrn` Rename a container
- `dks` Start one or more stopped containers
- `dkS` Restart a container
- `dkss` Display a live stream of container(s) resource usage statistics
- `dksv` Save one or more images to a tar archive (streamed to STDOUT by default)
- `dkt` Tag an image into a repository
- `dktop` Display the running processes of a container
- `dkup` Update configuration of one or more containers
- `dkV` Manage Docker volumes
- `dkv` Show the Docker version information
- `dkw` Block until a container stops, then print its exit code<Paste>
- `dkx` Stop a running container

#### container (C)

- `dkC` Manage containers
- `dkCa` Attach to a running container
- `dkCcp` Copy files/folders between a container and the local filesystem
- `dkCd` Inspect changes on a container's filesystem
- `dkCe` Run a command in a running container
- `dkCE` Run an interactive command in a running container
- `dkCin` Display detailed information on one or more containers
- `dkCk` Kill one or more running containers
- `dkCl` Fetch the logs of a container
- `dkCL` Fetch and follow (`-f`) the logs of a container
- `dkCls` List containers
- `dkCp` Pause all processes within one or more containers
- `dkCpr` Remove all stopped containers
- `dkCrn` Rename a container
- `dkCS` Restart one or more containers
- `dkCrm` Remove one or more containers
- `dkCr` Run a command in a new container
- `dkCR` Run an interactive command in a new container and automatically remove the container when it exits
- `dkCRe` like `dkCR` and set entry point to `/bin/bash`
- `dkCs` Start one or more stopped containers
- `dkCss` Display a live stream of container(s) resource usage statistics
- `dkCx` Stop one or more running containers
- `dkCtop` Display the running processes of a container
- `dkCP` Unpause all processes within one or more containers
- `dkCup` Update configuration of one or more containers
- `dkCw` Block until one or more containers stop, then print their exit codes

#### image (I)

- `dkI` Manage images
- `dkIb` Build an image from a Dockerfile
- `dkIh` Show the history of an image
- `dkIim` Import the contents from a tarball to create a filesystem image
- `dkIin` Display detailed information on one or more images
- `dkIls` List images
- `dkIpr` Remove unused images
- `dkIpl` Pull an image or a repository from a registry
- `dkIph` Push an image or a repository to a registry
- `dkIrm` Remove one or more images
- `dkIsv` Save one or more images to a tar archive (streamed to STDOUT by default)
- `dkIt` Tag an image into a repository

#### volume (V)

- `dkV` Manage volumes
- `dkVin` Display detailed information on one or more volumes
- `dkVls` List volumes
- `dkVpr` Remove all unused volumes
- `dkVrm` Remove one or more volumes

#### network (N)

- `dkN` Manage networks
- `dkNs` Connect a container to a network
- `dkNx` Disconnects a container from a network
- `dkNin` Displays detailed information on a network
- `dkNls` Lists all the networks created by the user
- `dkNpr` Remove all unused networks
- `dkNrm` Deletes one or more networks

#### system (Y)

- `dkY` Manage Docker
- `dkYdf` Show docker filesystem usage
- `dkYpr` Remove unused data

#### stack (K)

- `dkK` Manage Docker stacks
- `dkKls` List stacks
- `dkKps` List the tasks in the stack
- `dkKrm` Remove the stack

#### swarm (W)

- `dkW` Manage Docker Swarm

### Docker Machine

- `dkm` is short for `docker-machine`
- `dkma` Get or set the active machine
- `dkmcp` Copy files between machines
- `dkmd` Set up the default machine ; alowing you to use `dkme` without arguments
- `dkme` Set up the environment for the Docker client (eg: `dkme staging` to toggle to staging)
- `dkmin` Inspect information about a machine
- `dkmip` Get the IP address of a machine
- `dkmk` Kill a machine
- `dkmls` List machines
- `dkmpr` Re-provision existing machines
- `dkmps` is alias for `dkmls`
- `dkmrg` Regenerate TLS Certificates for a machine
- `dkmrm` Remove a machine
- `dkms` Start a machine
- `dkmsh` Log into or run a command on a machine with SSH
- `dkmst` Get the status of a machine
- `dkmS` Restart a machine
- `dkmu` Get the URL of a machine
- `dkmup` Upgrade a machine to the latest version of Docker
- `dkmv` Show the Docker Machine version or a machine docker version
- `dkmx` Stop a machine

### Docker Compose

> Note from docker-compose v1.29.2:
> Except for the Linux platform, Docker Compose is now in the Docker CLI.

- `dkc` is short for `docker-compose`
- `dkcb` Build or rebuild services
- `dkcB` Build or rebuild services and do not use cache when building the image
- `dkccp` Copy files/folders between a service container and the local filesystem
- `dkccr` Creates containers for a service
- `dkccv` Converts the compose file to platform's canonical format
- `dkcd` Stop and remove containers, networks, images, and volumes
- `dkce` Execute a command in a running container
- `dkcev` Receive real time events from containers
- `dkci` List images used by the created containers
- `dkck` Kill containers
- `dkcl` View output from containers
- `dkcL` View and follow (`-f`) output from containers
- `dkcls` List running compose projects (or alias to `dkcps` under Linux)
- `dkcp` Pause services
- `dkcP` Unpause services
- `dkcpl` Pull service images
- `dkcph` Push service images
- `dkcpo` Print the public port for a port binding
- `dkcps` List containers
- `dkcr` Run a one-off command
- `dkcR` Run a one-off command and remove container after run.
- `dkcrm` Remove stopped containers
- `dkcs` Start services
- `dkcsc` Set number of containers for a service
- `dkcS` Restart services
- `dkct` Display the running processes
- `dkcu` Create and start containers
- `dkcU` Create and start containers in detached mode:
           Run containers in the background, print new container names
- `dkcv` Show the Docker-Compose version information
- `dkcx` Stop services

## Author

*The author of this module should be contacted via the [issue tracker][3].*

- [François Vantomme](https://github.com/akarzim)

[1]: https://www.docker.com/
[2]: https://github.com/zplug/zplug
[3]: https://github.com/akarzim/zsh-docker-aliases/issues
[4]: https://github.com/zdharma-continuum/zinit
