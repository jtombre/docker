# docker

# Installing docker on Windows 10 Ubuntu

Reference: https://docs.docker.com/engine/installation/linux/ubuntulinux/

## Update your apt sources
 $ sudo apt-get update
 $ sudo apt-get install apt-transport-https ca-certificates

## Add the new gpg key
 $ sudo apt-key adv \
               --keyserver hkp://ha.pool.sks-keyservers.net:80 \
               --recv-keys 58118E89F3A912897C070ADBF76221572C52609D

## Add the docker repo
 $ sudo "deb https://apt.dockerproject.org/repo ubuntu-trusty main" | sudo tee /etc/apt/sources.list.d/docker.list

## Update repos
 $ sudo apt-get update

## Verify APT is pulling from the right repo
 $ apt-cache policy docker-engine

## Install 
 $ sudo apt-get install docker-engine

## Verify install
 $ sudo-cache policy docker-engine
