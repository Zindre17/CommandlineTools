# CommandlineTools
How to use different commandline tools (cheetsheet)

## Tables of Content
* [scp](https://github.com/Zindre17/CommandlineTools#scp-used-for-transfering-files-through-ssh)

## scp (used for transfering files through ssh)
typical usage: `scp fileToTransfer.extension username@ip:targetdirectory`

optional parameters:
* `-1`  Forces scp to use protocol 1.
* `-2`  Forces scp to use protocol 2.
* `-4`  Forces scp to use IPv4 addresses only.
* `-6`  Forces scp to use IPv6 addresses only.
* `-B`  Selects batch mode (prevents asking for passwords or passphrases).
* `-C`  Compression enable. Passes the -C flag to ssh to enable compression.
* `-c cipher` Selects the cipher to use for encrypting the data transfer. This option is directly passed to ssh.
* `-F ssh_config` Specifies an alternative per-user configuration file for ssh. This option is directly passed to ssh.
* `-i identity_file` Selects the file from which the identity (private key) for public key authentication is read. This option is directly passed to ssh.
* ` -l limit` Limits the used bandwidth, specified in Kbit/s.
* `-o ssh_option` Can be used to pass options to ssh in the format used in ssh_config. This is useful for specifying options for which there is no separate scp command-line flag.
* `-P port` Specifies the port to connect to on the remote host. Note that this option is written with a capital 'P', because -p is already reserved for preserving the times and modes of the file in rcp.
* `-p` Preserves modification times, access times, and modes from the original file.
* `-q` Quiet mode: disables the progress meter as well as warning and diagnostic messages from ssh.
* `-r` Recursively copy entire directories. Note that scp follows symbolic links encountered in the tree traversal.
* `-S program` Name of program to use for the encrypted connection. The program must understand ssh(1) options.
* `-v` Verbose mode. Causes scp and ssh(1) to print debugging messages about their progress. This is helpful in debugging connection, authentication, and configuration problems.
