# Ansible role for GIT
Ansible role for GIT 2.9 installation for CentOS 7

## What's inside?
1. GIT 2.9 and it's dependencies:
    - dh-autoreconf
    - curl-devel
    - expat-devel
    - gettext-devel
    - openssl-devel
    - perl-devel
    - zlib-devel
    - asciidoc
    - xmlto
    - docbook2X
    - getopt
2. Custom settings as per `defaults/main.yml`
   
## Tested on

## Installation
1. Navigate to Ansible's roles folder
2. Add the repo to git modules
    ```
    git submodule add https://github.com/budnerp/ansible_role_git.git ansible_role_git
    ```
3. Add the role to Ansible's playbook file
    ```    
    roles:
    [...]
        - ansible_role_git
    [...]
    ```
4. SSH into the VM instance. Execute:
    ```
    vagrant ssh
    ```
5. Setup GIT config
    ```
    $ git config --global user.name "John Doe"
    $ git config --global user.email johndoe@example.com
    ```
6. Validate config
    ```
    git config --list
    ```

## Other links
- Git [https://git-scm.com/]()
- Git tarballs list [https://mirrors.edge.kernel.org/pub/software/scm/git/]()
- Getting Started - Installing Git [https://git-scm.com/book/en/v2/Getting-Started-Installing-Git]()

## TO DO
-[ ] add dependencies 

## License
Copyright (c) We Are Interactive under the MIT license.