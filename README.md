# Infrastructure

This repository contains the files and descriptions to setup the infrastructure for [Emissions API](https://emissions-api.org/).

## Setup

### Prerequisites

This setup should be used on AWS with [Amazon Linux 2](https://aws.amazon.com/amazon-linux-2/).

For a nearly full automated setup we are using [Ansible](https://www.ansible.com/).

### Installation

First run the `user.yml` playbook to create the administrative user on the host.

After that you can run the `setup.yml` which bundles the remaining playbooks.
You need to have access to the vault for that.

It should also be possible to run a single playbook like `nginx.yml`,
if you have made some small changes and do not want to wait for the whole `setup.yml` to complete.
