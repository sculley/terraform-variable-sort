# terraform-variable-sort

This is a simple script to sort the variables in a Terraform file alphabetically. It's useful for keeping the variables in a file in a consistent order. By default it will look for a file called `variables.tf` in the current directory, but you can specify a different file as the first argument.

## Requirements

This script requires GNU `awk` which is available on most Linux distributions. You will need to install it on macOS using Homebrew or MacPorts.

```bash
brew install gawk
```

## Usage

```bash
./terraform-variable-sort.sh
```

## License

This project is licensed under the Apache License 2.0 - see the [LICENSE](LICENSE) file for details

## Authors

Module is maintained by [Sam Culley](https://github.com/sculley)