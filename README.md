# Various Shell Scripts

### About Shell Scripts

Shell scripts are basically a bunch of commands, which could theoretically also be entered line-by-line. Shell scripts bundle those commands together.

### Using Shell Scripts

There are various ways of using shell scripts. For this example, let’s assume our script is called `scriptName.sh`.

If the shell script file is not set to be executable, navigate to the directory of the script, and run

	./scriptName.sh

If the shell script _is_ executable, navigate to the directory of the script and run

	scriptName.sh

A script can be changed to be executable by using

	chmod +x scriptName.sh

----

Another way of using a shell script is assigning an `alias`. To find out how an alias can be assigned, you need to know which shell you’re running:


### Your Shell

The Shell is the user interface your Terminal uses in order to control the computer (here, we are talking about he command line, but for example the Finder in macOS is also a kind of Shell). There are various common command line shells. To find out wich shell you’re using, run

	echo $0

Common shells are `zsh` and `bash`.

Depending on the shell you’re running, you will need to edit the file `.zshrc` or `.bash_profile` (both those files are invisible files found in your user folder).
If the respective file does not exist, it needs to be created.

Within the file, an alias can be added like this:

	alias myFavoriteShellScript="/Users/USERNAME/code/scriptName.sh"

Make sure to use the acutual location of the script, as well as the proper user name. The full path to a file is easily retrieved (on macOS) using cmd-option-C

If we were to add an alias for `normalizeAll.sh`, this would be enough:

	alias normall='/Users/USERNAME/code/_AdobeTypeTools/shell-scripts/normalizeAll'

Note that the user name and location of the shell script will differ on a per-machine basis.
