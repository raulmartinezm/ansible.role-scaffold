# Vagrant boxes

## Usage

Show available boxes:

		$ vagrant status

Start a vagrant machine:

		$ vagrant up trusty64

or

		$ vagrant up centos7
	

Roles to apply can be specified in an environment variable:

		$ ANSIBLE_TAGS="myrole_tag" vagrant up trusty64
