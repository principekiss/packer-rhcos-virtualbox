# packer-rhcos-virtualbox

A Packer recipe for creating a RedHat CoreOS Vagrant box

## Required
- Packer
- VirtualBox
- Vagrant Cloud account
- Vagrant Cloud API key ([see here](https://www.vagrantup.com/vagrant-cloud/api#example-request))

Before running the packer build, you'll need to create a box on your Vagrant Cloud account with the same `version` and `box_tag` as specified in the `template.json`.
No need to add a provider, this will be pushed automatically with the box.

## Run
- Assign your Vagrant Cloud API key to `VAGRANT_CLOUD_TOKEN` environment variable.
- Run `packer build template.json`
