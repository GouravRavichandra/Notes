# CRAFT Installation

## Requirements 

- `Chocolatey`
- `Docker`
- `wsl`
- `ddev`


## Steps to initilize a project

Turn on Docker

Move inside the project working directory

`ddev config --project-type=craftcms --docroot=web --create-docroot`

`ddev composer create -y --no-scripts craftcms/craft`

`ddev craft install`

Add creds

`ddev launch`

TO stop the container - `ddev stop`
To start the container - `ddev `