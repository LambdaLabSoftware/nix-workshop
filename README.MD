# Nix workshop 

We're going to follow https://zero-to-nix.com

Nix quickstart guide to get the basics in place


# Installing Nix onon a ubuntu base docker image using Determinate Systems

```bash
# Building the image locally 
docker build -t nix-on-docker nix-on-docker
# Test if the image works
docker run -it nix-on-docker nix run nixpkgs#ponysay -- "Hi"
# Run an interactive bash shell(if you close the shell the nix cache will be nvalidated so recommended to work in this shell for the workshop)
docker run -it nix-on-docker bash