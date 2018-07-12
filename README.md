# PXVM
A basic Prince XML version manager

## Installation
- Clone the repository into the directory of your choosing
- Move to the cloned directory
- _Optional_: If you want to explicitly determine which profile to install the path shim in , you can set the `PROFILE` variable before using the install script (e.g. `PROFILE=path/to/my/profile`).
- Run command `source ./script/install`
- Then either restart your shell or run `source ./script/instant_shim`
- Try `pxvm` to test that the installation was successful

**Note:** If you are a OSX user on a Bash shell and your system cannot find the `pxvm` command after a shell restart, try adding `source ${HOME}/.bashrc` to `.bash_profile` in your home directory. As a one-liner, you can run: `echo -e "\nsource \${HOME}/.bashrc" >> ${HOME}/.bash_profile`

**Note:** The `pxvm` command itself is installed on a per-shell basis. If you change what shell you are using, then you will need to run the installation script again. Re-running the install script will not wipe your added Prince XML versions.

## Usage
Commands:
- `pxvm h|help`
  - Show help message
- `pxvm v|version`
  - Show version
- `pxvm a|add <name> <source>`
  - Add a Prince XML version to PXVM and name it <name>
  - Note: \<source\> must be a path to a `.tar.gz` Prince XML package, such as those available on the [Prince XML site](https://www.princexml.com/download/)
- `pxvm l|list`
  - List all added and named Prince XML versions
- `pxvm s|system`
  - Use the system installed Prince XML
- `pxvm u|use <name>`
  - Use a previously added and named Prince XML version
### Sample Usage
```
$pxvm list
Available Prince Versions:
None
$pxvm add v11 path/to/princev11.tar.gz
Added Prince XML version with name v11
$pxvm list
Available Prince Versions:
v11
$pxvm use v11
Now using Prince XML with name v11
```
