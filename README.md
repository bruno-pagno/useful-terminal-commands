# Useful terminal commands


## General
```bash
# List any process listening to a port
lsof -i:PORT

# Kill any process listening to the port
kill $(lsof -t -i:PORT)             
```

## Git
```bash
# Checkout to last git stash
$ git checkout stash@{0}

# Get a specific file from the last git stash
$ git checkout stash@{0} -- <filename>
```

## Docker
```bash
# Stop all docker containers
docker stop $(docker ps -a -q)         

# Remove all the containers
docker rm $(docker ps -a -q)
```