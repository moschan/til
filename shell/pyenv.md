# Installing pyenv virtual env using brew
brew install pyenv-virtualenv pyenv

# list of versions
pyenv install -l

# Installing specific version
pyenv install 2.7

# Checking local installed pythons
pyenv virtualenvs

# Creating working environmwnr
pyenv virtualenv [version] [name]

# Apply it on current directory
pyenv local [name]

# Uninstalling 
pyenv uninstall sandbox336
pyenv uninstall 3.3.6
