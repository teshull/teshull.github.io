I am using rvm to manage different ruby versions.

Currently I am using ruby 2.7.2

To set this, use the command: "rvm use ruby-2.7.2"

Note for this to work you may have to follow the "/bin/bash --login" prompt

on mac you can do the following

export PATH="/opt/homebrew/opt/ruby@2.7/bin:$PATH


If you need to have ruby@2.7 first in your PATH, run:
  echo 'export PATH="/opt/homebrew/opt/ruby@2.7/bin:$PATH"' >> ~/.zshrc

For compilers to find ruby@2.7 you may need to set:
  export LDFLAGS="-L/opt/homebrew/opt/ruby@2.7/lib"
  export CPPFLAGS="-I/opt/homebrew/opt/ruby@2.7/include"
