# Ansible Version Manager

Auto detect per project the correct version of Ansible to run.

## How does it work?
1. Create in your project a single `.avm` file with the Ansible version this project requires to run i.e. `2.4.0.0`
2. It will auto detect within a terminal if your current installation of Ansible is correct if not it'll prompt you to create a virtual enviroment with that version of Ansible within it.


## Will it remove my current installed version?
No it will create a virtual environment within your terminal meaning that each terminal is unique allowing your to run different versions of Ansible per terminal session.


## Pre requisites
1. Please have pip installed.
2. Please have git installed.


## Installation
1. Clone the git repo
2. run `chmod a+x avm`
3. run `avm install`


## Once installed what is next?
1. Create in your project a `.avm` file with the Ansible version required for the project i.e. `2.4.0.0`
2. When you cd into the directory that contains a `.avm` it will warn if the current version of Ansible does not match the project requirements
3. Run `. avm use` and this will create a virtual environment with the correct version of Ansible to use 
