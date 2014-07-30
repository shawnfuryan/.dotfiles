dotfiles
========
These are common configuration files that I use.

IMPORTANT! Before filling out any of the authentication
credential lines in the dotfiles/secrets directory, it is
important to restrict read access on this directory and
the files contained in it. This can be achieved with the
following line (assuming the dotfiles directory is
located at ~/dotfiles)

> chmod 600 ~/.dotfiles/secrets && chmod 600 ~/.dotfiles/secrets/*

Also, this repository is meant to be maintained locally
after an intial clone. DO NOT PUSH to a public git repo
after adding sensitive information like API keys or
passwords.

The way that I do it is to clone the .dotfiles repo to the local
machine in a projects directory, and then move the files in the 
repo to the user directory that I want to use them in. Something
like:

> cp -R ~/Projects/.dotfiles/ ~

Then I delete the hidden git directory

> rm -rf ~/.dotfiles/.git/

And populate the environment variables in ~/.dotfiles/secrets/*

This workflow allows me to track changes to the repository while
making it less likely that I will boneheadedly publish secrets.
