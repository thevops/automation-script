# Run - automation script in Bash

Quite good replecement for Makefile (example [here](https://github.com/thevops/makefile-automation))

Look at example file `run` in this repository.

Here is YouTube video with more information: https://www.youtube.com/watch?v=SdmYd5hJISM

## Fast start

1. Download `run` file
2. Put `alias run='./run'` to your `.zshrc`
3. Execute `source <(./run zsh_setup)` for auto-completion.

## Example

```
╰─❯ ./run

./run <task> [args]

Tasks:
	cmd                 	Run any command you want in the web container
	flask               	Run any Flask commands
	psql                	Connect to PostgreSQL with psql
	redis-cli           	Connect to Redis with redis-cli
	pip3:install        	Install pip3 dependencies and write lock file
	clean               	Remove cache and other machine generates files
	help                	Help menu
	zsh_setup           	For ZSH auto-completion: source <(./run zsh_setup)

Extended help:
  Each task has comments for general usage

Task completed in 0m0.008s
```

## Credits

> I'm not author of this script. I only made some changes for ZSH.

- https://github.com/adriancooney/Taskfile
- https://github.com/nickjj/docker-flask-example/blob/main/run
