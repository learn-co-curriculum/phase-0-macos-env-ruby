# Installing Ruby on MacOS

## Install the GMP and GnuPG Packages

Before installing RVM and Ruby, we will need to add two tools which help us to
verify that we're installing the software that we're expecting.

### Action Item

1. Open the "Terminal" application using "Spotlight Search"
2. Type `brew install gmp` and press `<Enter>`
3. Type `brew install gnupg` and press `<Enter>`

### Check Your Work

<iframe width="560" height="315" src="https://www.youtube.com/embed/5JTWcR7n1xo" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

If you get an error saying "command not found: brew", Homebrew may not be
installed or failed to install correctly. Please go back through the "MacOS
System Setup" lesson first before going through the rest of this one.

If you get an error saying "Warning: gnupg-1.4.19 already installed", GnuPG is
installed, but it may not be linked properly. To fix:

1. Open the "Terminal" application using "Spotlight Search"
2. Type `brew link gnupg` and press `<Enter>`

## Install Ruby Environment Manager (RVM) on macOS

[Ruby Environment Manager (RVM)][rvm] is a tool that will allow you to download
and install multiple versions of Ruby, one of the programming languages that we
teach at Flatiron School. This is the first step in installing Ruby on your
macOS operating system.

[rvm]: https://rvm.io/

### Action Item

1. Open the "Terminal" application using "Spotlight Search"
2. Type
   `gpg --recv-keys 409B6B1796C275462A1703113804BB82D39DC0E3 7D2BAF1CF37B13E2069D6956105BD0E739499BDB`
   and press `<Enter>`
3. Type `\curl -sSL https://get.rvm.io | bash -s stable` and press `<Enter>`
4. Close and reopen the "Terminal" application
5. Type `rvm` and press `<Enter>`

### Check Your Work

<iframe width="560" height="315" src="https://www.youtube.com/embed/KLPVQDUYu-I" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

If you see a long message ending in "For additional documentation please visit
https://rvm.io", continue below.

If `rvm` is not found, check out the troubleshooting steps in the **Verify and
Troubleshoot your macOS Environment Setup** lesson later on in this module.

## Install Ruby version 2.7.4 on macOS

For our Ruby labs and lessons, we expect that students use Ruby version 2.7.4.
If Ruby Environment Manager (RVM) has been successfully installed, you can
quickly install Ruby with a couple of commands.

### Action Item

1. Open the "Terminal" application using "Spotlight Search"
2. Type `rvm install 2.7.4 --default` and press `<Enter>`
3. Type `rvm list` and press `<Enter>`

### Check Your Work

<iframe width="560" height="315" src="https://www.youtube.com/embed/cKU3o2xqqtU" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

If you see a message starting with "=\* ruby-2.7.4", continue below.

## Install Ruby Gems

Ruby Gems are small programs written in Ruby that help you to code more easily
in Ruby. The gems you will install today include: Bundler, which allows you to
keep track of which gems your projects need to work, and Pry, which allows you
to pause Ruby code execution when it runs and inspect it.

### Action Item

1. Open the "Terminal" application using "Spotlight Search"
2. Type `gem update --system` and press `<Enter>`
3. Type `gem install bundler` and press `<Enter>`
4. Type `gem install pry` and press `<Enter>`
5. Type `gem list | wc -l` and press `<Enter>`

### Check Your Work

<iframe width="560" height="315" src="https://www.youtube.com/embed/rc5vn4FVvXc" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

If you can complete each step without any issues and you see an output of a
number around or above 60 from the last command, continue to the next lesson,
**Configuring Git and GitHub on macOS**.
