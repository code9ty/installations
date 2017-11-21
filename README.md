# Installing rails
1. Install curl

    If you are running Ubuntu or any debian based distro run

    `sudo apt-get install curl`

2. Install rvm then ruby

***NB: Don't forget to install the keys from https://rvm.io otherwise this won't work*** 

    `$ gpg --keyserver hkp://keys.gnupg.net --recv-keys 409B6B1796C275462A1703113804BB82D39DC0E3 7D2BAF1CF37B13E2069D6956105BD0E739499BDB`
    `$ \curl -L https://get.rvm.io | bash -s stable --ruby`

3. Run command as login

    Follow [this link](https://rvm.io/integration/gnome-terminal#integrating-rvm-with-gnome-terminal) to enable this feature then restart your terminal before proceeding

4. Install nodejs

    `sudo apt-get install nodejs`

5. Install nokogiri and bundler gems

    `rvm gemset list`

    confirm that global and default gemsets are present

    `rvm gemset use global`

    `$ echo "gem: --no-document" >> ~/.gemrc`

    `gem install bundler`

    `gem install nokogiri`

6. If you planing on using postgresql on local machine

    `sudo apt-get install libpq-dev`

    `gem install pg`

7. Install rails

   `gem install rails`

8. Create new rails application

    Create directory to hold your code

    `mkdir code`
    
    cd into the directory

    `cd code`

    `mkdir myapp`

    `cd myapp`

    `rvm use ruby-2.x.x@rails5.0 --ruby-version --create`

    Create new rails app

    `rails new .`

# Installing vim.

We can use a version that is already setup with plugins necessary to kick us off

On your command prompt run the following command

`curl http://j.mp/spf13-vim3 -L -o - | sh`

For more on customization and how to setup more plugins visit the official site 
[here](http://vim.spf13.com/)

Be patient while vim installs

If you do not have prior experience with vim, type `vimtutor` on your terminal to have a brief
interactive tutorial
