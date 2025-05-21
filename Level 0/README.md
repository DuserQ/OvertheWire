![Alt text](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fthanoskoutr.com%2Fcovers%2Foverthewire.jpg&f=1&nofb=1&ipt=0baeec90a558310488c80a6f9fe93fdc6571e3a1f818fa72ce7b6fbbb425a623)
## Level Description
The goal of this level is for you to log into the game using SSH. The host to which you need to connect is bandit.labs.overthewire.org, on port 2220. The username is bandit0 and the password is bandit0. Once logged in, go to the Level 1 page to find out how to beat Level 1.

## Analysis
the problenm said that to solve the challenge the only thing we need is to connect the address and the port that gave us. the command the we gonna use is the mention before, `ssh`.

we gonna say that `ssh` is one of the most important tools that have the terminals, because help us connect in a securely way to a remote server through the internet.

knowing that, let's see how it works, in our terminal we gonna write this command:
```bash
$ man ssh
```
the `man` command is the manual for the specified command that we put in front of him. in this case is `ssh`.
after pressing enter the respective manual its gonna deploy in our terminal
```bash
SSH(1)                                                                                                   General Commands Manual                                                                                                  SSH(1)

NAME
       ssh — OpenSSH remote login client

SYNOPSIS
       ssh  [-46AaCfGgKkMNnqsTtVvXxYy]  [-B  bind_interface]  [-b  bind_address]  [-c  cipher_spec] [-D [bind_address:]port] [-E log_file] [-e escape_char] [-F configfile] [-I pkcs11] [-i identity_file] [-J destination] [-L address]
           [-l login_name] [-m mac_spec] [-O ctl_cmd] [-o option] [-P tag] [-p port] [-R address] [-S ctl_path] [-W host:port] [-w local_tun[:remote_tun]] destination [command [argument ...]]
       ssh [-Q query_option]

DESCRIPTION
       ssh (SSH client) is a program for logging into a remote machine and for executing commands on a remote machine.  It is intended to provide secure encrypted communications between two untrusted hosts over an insecure  network.
       X11 connections, arbitrary TCP ports and Unix-domain sockets can also be forwarded over the secure channel.

       ssh  connects and logs into the specified destination, which may be specified as either [user@]hostname or a URI of the form ssh://[user@]hostname[:port].  The user must prove their identity to the remote machine using one of
       several methods (see below).

       If a command is specified, it will be executed on the remote host instead of a login shell.  A complete command line may be specified as command, or it may have additional arguments.  If supplied, the arguments  will  be  ap‐
       pended to the command, separated by spaces, before it is sent to the server to be executed.
```





