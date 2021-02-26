# Localenv Builder Installer

This repo contains the installer for the Konsentus Local Development environment.

The actual builder is in the repo: https://github.com/Konsentus/localenv-builder

## Prerequisites

You should have git installed and a ssh key created to allow you to access Konsentus private repositories.

## Installing the Build Tool

1. Run `sudo mkdir -p /usr/local/{var,bin} && sudo chown $(whoami) /usr/local/*`
2. Run `xcode-select --install` to ensure you have the latest xcode command line tools (if the command errors, you can install the tools manually from the [Engineering Team's OneDrive](https://konsentusltd.sharepoint.com/:f:/s/engineering-team2/EmNuvDCuKbFKkYAK_t3x18kBkA9HdxhHIKf39SnngntCFA?e=6zaesY))
3. Run `python3 -c "$(curl -s https://raw.githubusercontent.com/Konsentus/localenv-builder-installer/main/install)"`
4. Once the installation is complete you will need to switch to the custom iTerm profile. To do this, open iTerm, go to 'preferences' and select 'profiles'. Select 'LocalEnv Default' in the profile list and click 'Other Action...' -> 'Set as Default'. When iTerm is restarted, the new profile will be used.
