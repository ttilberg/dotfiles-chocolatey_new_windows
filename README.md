# dotfiles-chocolatey_new_windows
Install Chocolatey, and packages I want. Not a dotfile, but relevant to getting a "fresh computer" up an running.

This is just a place to maintain packages I probably want installed on a fresh Windows machine.

[Chocolatey](https://chocolatey.org) is a package manager for Windows, akin to using apt-get, or homebrew.

```
###
# Install Chocolatey (see https://chocolatey.org )
# Admin CMD
@powershell -NoProfile -ExecutionPolicy Bypass -Command "iex ((new-object net.webclient).DownloadString('https://chocolatey.org/install.ps1'))" && SET PATH=%PATH%;%ALLUSERSPROFILE%\chocolatey\bin

###
# Packages
#   These can be combined into a statement such as 
#     choco install chrome skype dropbox
#   but they are being listed individually for easy copy/paste

# General
choco install chrome
choco install skype
choco install dropbox

# Editors
choco install sublimetext3 sublimetext3.packagecontrol sublimetext3-contextmenu sublimetext3.powershellalias
choco install notepadplusplus
choco install visualstudiocode

# Programming Languages
choco install ruby
choco install python

# Programming Tools
choco install cmder
choco install git -params '"/GitAndUnixToolsOnPath"'
choco install virtualbox
choco install vagrant
choco install docker docker-machine


# Games
choco install steam
choco install minecraft



```
