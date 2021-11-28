# Personal config

## Introduction

This repo's goal is to contain my personal configuration for the software tools I'm using.
For now, there is configuration for:
    - git
    - vim
    - zsh

All those configuration are stored so they can be installed using ansible.
When installing with ansible, symbolic links to the configurations files found in the repo will be created.
This allow this repo to be easily updated in case of any changes in the personal config (new commit to the repo et voilà).

## How to use ansible
To install the configuration using ansible you need:
    - To install ansible
    - To change directory to be in .personal_configs
    - To run: ansible-playbook -i inventory -K system_setup.yml

After running the command, you will be asked for a password.
Enter your sudo password.

The inventory file contains the list of the machine to apply the configuration to.
Don't hesitate to create your own.
