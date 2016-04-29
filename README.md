# docker-ubuntu-ppa-build
Contains devscripts and debhelper for pushing packages to ppas

# Usage

In the directory where your build files are run

`docker run -ti --rm -v $HOME/.gnupg:/root/.gnupg:ro -v $PWD:/target rwky/docker-ubuntu-ppa-build bash`

This will drop you into a bash shell where you can run your build script, it mounts your gpg directory so you can sign packages. Your files will be in /target
