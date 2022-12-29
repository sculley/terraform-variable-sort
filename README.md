# terraform-variable-sort

This is a simple script to sort the variables in a Terraform file alphabetically. It's useful for keeping the variables in a file in a consistent order. By default it will look for a file called `variables.tf` in the current directory, but you can specify a different file as the first argument.

## Requirements

This script requires GNU `awk` which is available on most Linux distributions. You will need to install it on macOS using Homebrew or MacPorts.

```bash
brew install gawk
```

## Installation

Install the script using Homebrew

```bash
brew tap sculley/homebrew-formula
brew install terraform-variable-sort
```

## Usage

### Homebrew

```bash
terraform-variable-sort
```

Specify a different file as the first argument.

```bash
terraform-variable-sort variables.tf
```

### Manual

```bash
curl -s https://raw.githubusercontent.com/sculley/terraform-variable-sort/main/terraform-variable-sort.sh | bash -s --
```

Specify a different file as the first argument.

```bash
curl -s https://raw.githubusercontent.com/sculley/terraform-variable-sort/main/terraform-variable-sort.sh | bash -s -- input.tf
```

Your file will be updated in place.

## License

This project is licensed under the Apache License 2.0 - see the [LICENSE](LICENSE) file for details

## Authors

Module is maintained by [Sam Culley](https://github.com/sculley)

## Acknowledgments

The AWK script was taken from [Github Gist](https://gist.github.com/yermulnik/7e0cf991962680d406692e1db1b551e6)

This script was adapted from [libre-devops/utils/tf-sort.sh](https://github.com/libre-devops/utils/blob/dev/scripts/terraform/tf-sort.sh)