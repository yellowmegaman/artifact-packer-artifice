# Hashicorp Packer artifice post-processor example

What it does:
- spin GCE instance
- install docker
- run packer template to create docker container
- save to tar
- download
- compress

Sad thing that image discard flag non-existent, so there's always gonna be image left after build.
Can still be used in environments where access to docker daemon is limited, or artifact can only be built in specific environment.
