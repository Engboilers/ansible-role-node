# Ansible Role: Node

[![Build Status](https://travis-ci.org/engboilers/ansible-role-node.svg?branch=master)](https://travis-ci.org/engboilers/ansible-role-node)

Installs node and global npm packages.

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    node_versions: []

Node versions you would like to make sure are installed by nodenv.

    node_npm_global_packages: []

Global NPM packages you would like to make sure are installed.

## Dependencies

  - `engboilers.homebrew`

## Example Playbook

    - hosts: localhost
      roles:
        - { role: engboilers.node, node_execute: true }

## License

Apache 2.0
