--- Initializing a Linux System ---

sudo apt-get update -y && apt-get dist-upgrade -y
# Install ZSH
sudo apt-get install zsh
# Robbyrussell Install Script to initialize ZSH and change the shell.
./zshinit.sh
# Add in plugins to ZSH : 
#plugins=(git autojump autopep8 brew common-aliases extract git-extras github 
#         npm node pip python repo sublime command-not-found)
# You can edit them in .zshrc file.
# Install an anonmizer 
sudo apt-get install kalitorify | kalitorify -s
# Fetch all the Repositories from Git using Gitim.
cd gitim | python -m gitim -u
# Install ATOM Editor : https://flight-manual.atom.io/getting-started/sections/installing-atom/
# Once the ATOM Editor is installed Change your Theme using Atom package Manager.
apm install predawn-syntax
# Install Python language server [python -m pip install 'python-language-server[all]']
python -m pip install 'python-language-server[all]'
# Install all the packages required for python programming.
# Python ide support for Atom
# File Icon Package
# Script Package : https://atom.io/packages/script
apm install script
apm install atom-file-icons
apm install ide-python
apm install atom-ide-ui


