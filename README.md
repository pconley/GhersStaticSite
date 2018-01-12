# Ghers Static Site
- docker (must be installed)
- apache (is not required... docker builds it)
- the conf file is not used (todo to remove it)
- restart.sh 
  - has all the commands to build, start and stop the container.
  - careful as it stops and removes ANY docker container running.

## Instructions
Clone this repo
```
. ./restart.sh
```
Access at localhost:8080 (or was it 80... i forget)

Please update me (the readme) if you see any issues.

## Notes
I did not mount a volume in the docker image, tha means that every time I make a change
to the code I have to rebuild the image (via restart) in a bigger project a shared 
volume would fix that... but I wanted the docker image here to conatin the actual code.
