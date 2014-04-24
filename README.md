# nSSH for Emacs

nssh is a new SSH mode for Emacs. It takes some inspiration and code
from `ssh-mode`.

## Features

 - Based on TRAMP and shell-mode, can log into any host TRAMP can,
   including proxied hosts (bastion, sudo, etc)
 - History ring of hosts logged into
 - Tab completion of hosts in history and `known_hosts`
 - Tab completion in the remote shell
 - Lightweight & simple

## Installation

Copy `nssh.el` somewhere in your `load-path` and `(require 'nssh)`.

## Usage

`M-x nssh RET` will open a connection. If a live connection is open,
it will be brought to the foreground. If the buffer exists, but the
process is dead, it will reconnect. With a prefix argument, opens a
new connection.
