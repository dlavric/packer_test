# packer_test

## What this is

This repository is for creating an AMI that contains the latest version on Nginx.

For configuration of Nginx on Ubuntu, please see https://www.digitalocean.com/community/tutorials/how-to-install-nginx-on-ubuntu-20-04

## Working with this repository

Pre-requisites:
1. [AWS Credentials.](https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-install.html)
2. [Packer](https://learn.hashicorp.com/tutorials/packer/get-started-install-cli)

## How to Use the Repo
- Clone this repo:
```shell
 git clone git@github.com:dlavric/packer-base.git
```

- Go to the directory where the repo is stored
```shell
 cd packer-base
```

- To build the image simply run
```shell
packer init
```
    and
```shell
packer build
```

Since this is using a base AMI from AWS, it will require AWS access to pull the generic AMI as well as build the new AMI and push it.
