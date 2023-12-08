# CRAFT Installation

## Requirements 

- `Chocolatey`
- `Docker`
- `wsl`
- `ddev`


## Steps to initilize a new project

Turn on DockerDesktop with `ddev` installed

Move inside the project working directory

  - `ddev config --project-type=craftcms --docroot=web --create-docroot`
  - `ddev composer create -y --no-scripts craftcms/craft`
  - `ddev craft install`
  - Add creds
  - `ddev launch`
  - To stop the container - `ddev stop`.
  - To start the container - `ddev `.

## Steps to initilize an existing craftcms project

  - run `ddev config`.
  - follow the steps on the screen.
  - run `ddev start` to start the craftcms project.

### To install things, ssh into the ddev using `ddev ssh`.
  - Run all the necessary commands in the ssh window.
    This might show some errors as the scripts are in windows format and not in unix style.

### Using `ddev exec` followed by the command will help us run the code in windows using ddev env.
### Use `ddev exec php {commad}` to install in ddev. example - `./craft setup/security-key` can be written as `ddev exec php craft setup/security-key`
