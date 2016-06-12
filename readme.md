# Technologic Server Management

A collection of Ansible playbooks to install, update and management our
ubuntu 14.04 LTS server

## Python module

* pip install cryptography
* pip install passlib

## Creating a user

TODO: create a script.

If you don't have a user please create your new user with the 
_create-user_ playbook.

First you need to create a crypt password with the python and passlib module. 
Install the passlib module with ```pip install passlib```. Afterwards you can run 
the following code to create a password:

```
python2 -c "from passlib.hash import sha512_crypt; import getpass; print sha512_crypt.encrypt(getpass.getpass())"
```

The command will prompt you for a password and encrypts you input