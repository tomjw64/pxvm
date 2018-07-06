# PXVM
A basic Prince XML version manager

## Installation
- Clone the repository into the directory of your choosing
- Move to the cloned directory
- `source ./script/install`

## Usage
Commands:
- `pxvm h|help`
  - Show help message
- `pxvm a|add <name> <source>`
  - Add a Prince XML version to PXVM and name it <name>
  - Note: <source> must be a path to a `.tar.gz` Prince XML package, such as those available on the [Prince XML site](https://www.princexml.com/download/)
- `pxvm l|list`
  - List all added and named Prince XML versions
- `pxvm s|system`
  - Use the system installed Prince XML
- `pxvm u|use <name>`
  - Use a previously added and named Prince XML version
