# git-siktir

A git command to help you clean up your local branches.

# Installation

Simply copy the ```git-siktir``` file in a directory included in your ```$PATH```. For example:

```sh
$ sudo - su
# cp git-siktir /usr/local/bin
```

# Execution

To use the command execute the following command in the working directory you want to clean up:

```sh
$ git siktir
```

Currently there is only one mode supported, which is: detecting which of your local branches used to be tracking a remote branch, but do not track a remote any more. Those branches are saved in a file in ```/tmp``` and then the ```vi``` editor opens so you can review and curate the list. Save the file after making any changes and exit the editor. After exiting the editor the script will remove the branches still listed in the file.
