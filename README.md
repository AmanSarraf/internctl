# internsctl

`internsctl` is a command-line tool designed to perform various system operations. It provides functionalities related to CPU information, memory information, user management, and file information retrieval.

## Table of Contents
- [internsctl](#internsctl)
  - [Table of Contents](#table-of-contents)
  - [Installation](#installation)
    - [Options:](#options)
      - [Subcommands](#subcommands)
    - [Examples](#examples)
  - [Contributing](#contributing)
  - [License](#license)

## Installation

To use `internsctl`, follow these steps:

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/internsctl.git
   
```bash
cd internsctl
``````
```bash 
chmod +x internsctl
```
```bash
sudo mv internsctl /usr/local/bin/

```
```bash
internsctl [options] subcommand [arguments]

```

### Options:
- --help: Display help information.
- --version: Display the version of internsctl.
#### Subcommands
- cpu getinfo: Get CPU information (similar to lscpu).
- memory getinfo: Get memory information (similar to free).
- user create <username>: Create a new user with the given username.
- user list: List all regular users.
- user list --sudo-only: List users with sudo permissions.
- file getinfo [options] <file-name>: Get information about a file.
Options:
 --size, -s: Print file size.
 --permissions, -p: Print file permissions.
 --owner, -o: Print file owner.
 --last-modified, -m: Print last modified time of the file.

 ### Examples

 ```bash
 # Get CPU information
internsctl cpu getinfo

# Get memory information
internsctl memory getinfo

# Create a new user
internsctl user create newuser

# List all regular users
internsctl user list

# List users with sudo permissions
internsctl user list --sudo-only

# Get file size
internsctl file getinfo --size sample.txt

# Get file permissions
internsctl file getinfo --permissions sample.txt

# Get file owner
internsctl file getinfo --owner sample.txt

# Get last modified time of the file
internsctl file getinfo --last-modified sample.txt
```
## Contributing
If you'd like to contribute to this project, please follow the Contributing Guidelines.

## License
This project is licensed under the MIT License - see the LICENSE file for details.