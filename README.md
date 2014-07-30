dotfiles
========
These are common configuration files that I use.

IMPORTANT! Before filling out any of the authentication
credential lines in the dotfiles/secrets directory, it is
important to restrict read access on this directory and
the files contained in it. This can be achieved with the
following line (assuming the dotfiles directory is
located at ~/dotfiles)

> chmod 600 ~/dotfiles/secrets && chmod 600 ~/dotfiles/secrets/*

Also, this repository is meant to be maintained locally
after an intial clone. DO NOT PUSH to a public git repo
after adding sensitive information like API keys or
passwords.
