# docker-wrapper
Docker command wrapper.

> The `docker-wrapper` command is a **complete** superset of the `docker` command. It is a wrapper that shims the native `docker` command with useful aliases and helpers to enhance your docker workflow. This may go without saying, but `docker` is a required dependency for `docker-wrapper`.

### Installation
```bash
$ git clone "https://github.com/clarketm/docker-wrapper.git"

$ cd docker-wrapper && sh install.sh
```

### Usage
```bash
$ docker-wrapper wrapper --help
```

```text
NAME:
	docker-wrapper – docker command wrapper.


SYNOPSIS:
	docker-wrapper subcommand [opts...]


SUB COMMANDS:

	b, build                    	 Build an image from a Dockerfile.

	e, exec                     	 Run a command in a running container.
	    -b, --bash              	 Execute bash in a running container.
	    -i, --interactive       	 Execute command in interactive container.

	i, images                   	 List images.
	    -d, --dangling          	 List all dangling images.
	    -v, --verbose           	 List all images (non-truncated output).

	ip                          	 List IP address(es) for container.

	p, ps                       	 List containers.

	rm                          	 Remove one or more containers.
	    -a, --all               	 Remove all containers.
	    -e, --exited            	 Remove all exited containers.
	    -r, --running           	 Remove all running containers.

	rmi                         	 Remove one or more images.
	    -a, --all               	 Remove all base images.
	    -d, --dangling          	 Remove all dangling images.
	    -i, --intermediate      	 Remove all images (both base AND intermediate).

	r, run                      	 Run a command in a new container.
	    -i, --interactive       	 Run interactive container.

	s, stop                     	 Stop one or more running containers.
	    -a, --all               	 Stop all processes/containers.

	w, wrapper                  	 Docker wrapper specific options.
	    -h, --help              	 Print usage information.
	    -v, --version           	 Print version number.


MANAGEMENT COMMANDS:

	n, network                  	 Manage networks.

	v, volume                   	 Manage volumes.

	    ls                      	 List volumes.
	        -d, --dangling        	 List all dangling volumes.

	    rm                      	 Remove one or more volumes.
		-d, --dangling        	 Remove all dangling volumes.


EXAMPLES:
	docker-wrapper wrapper --help

```

### TODO (before official v1.0.0 release):
- [ ] Cross-platform compilation for Linux OS
- [ ] Add completions
