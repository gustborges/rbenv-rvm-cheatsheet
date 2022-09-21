# Rbenv & RVM Cheatsheet

```
# First we need to clean up previous ruby installations
rvm implode && sudo rm -rf ~/.rvm

# If you got "zsh: command not found: rvm", carry on. It means `rvm` is not
# on your computer, that's what we want!
sudo rm -rf $HOME/.rbenv /usr/local/rbenv /opt/rbenv /usr/local/opt/rbenv
brew uninstall --force rbenv ruby-build

# Quit the terminal, open another one and
brew instal rbenv

# Quit again and restart. Now, we can install the latest ruby version.
rbenv install 3.0.1 #takes 5 to 10 minutes

# Tell the system to use that version globally by default
rbenv global 3.0.1
#or local

# Restart the terminal again and check if it's updated
ruby -v


# RVM
# List known versions
rvm list known

# List versions that you have
rvm list

# Install a version
rvm install 3.0.0

# Check version
rvm -v
ruby -v

# Change version
rvm use 2.7.3

# Adapt gems (creates .ruby or .rvm file?)
rvm gemset create name-of-the-app
```
