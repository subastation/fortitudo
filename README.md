# fortitudo
Deploy your website in seconds, in a container 

This is an Ansible role that deploys two httpd containers with different logging paths based on their name and also deploys a website given a GitHub website compatible repository. This role is designed to work on a Linux machine with `dnf` package manager installed.

## Requirements

* Linux machines in inventory must run `dnf` package manager (or yum if you modify the role).

## Usage

To deploy your website in two httpd containers, follow these steps:

1. Clone this repository
2. Edit `vars/main.yaml` and `tests/inventory` for your environment
3. Run `tests/test.yaml`
    ```
    ansible-playbook -i tests/inventory tests/test.yaml
    ```
4. Verify that the containers and website are running as expected

