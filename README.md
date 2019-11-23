# PipUpdateAll

This utility allows you to quickly upgrade all outdated packages installed using `pip`.

## Command Line

The utility is called as: `pip_update_all`.  If you are using Windows, this will run a batch file that calls the utility using Python.

## How It Works

The utility first runs `pip` to gather a list of all outdated packages using the `pip list --outdated` command.  The output is captured to a string which is then parsed to produce a list of packages that require upgrading.  Each package in the list is upgraded by running the `pip install PACKAGE_NAME --upgrade` command, with the output displayed in the terminal.
