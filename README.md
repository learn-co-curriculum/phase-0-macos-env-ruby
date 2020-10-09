# Installing Ruby on macOS

## Install the GMP and GnuPG Packages

Before installing RVM and Ruby, we will need to add two tools which help us to
verify that we're installing the software that we're expecting.

### Action item

1. Open the "Terminal" application using "Spotlight Search"
2. Type `brew install gmp` and press `<Enter>`
3. Type `brew install gnupg` and press `<Enter>`

### Check Your Work

If you get an error saying "Warning: gnupg-1.4.19 already installed", GnuPG is
installed, but it may not be linked properly. To fix:

1. Open the "Terminal" application using "Spotlight Search"
2. Type `brew link gnupg` and press `<Enter>`

## Install Ruby Environment Manager (RVM) on Ubuntu

Ruby Environment Manager (RVM) is a tool that will allow you to download and
install multiple versions of Ruby, one of the programming languages that we
teach at Flatiron School. This is the first step in installing Ruby on your
Ubuntu operating system.

### Action Item

1. Open the "Terminal" application using "Spotlight Search"
2. Type `curl -sSL https://rvm.io/mpapis.asc | gpg --import -` and press `<Enter>`
3. Type `curl -sSL https://rvm.io/pkuczynski.asc | gpg --import -` and press `<Enter>`
4. Type `\curl -sSL https://get.rvm.io | bash` and press `<Enter>`
5. Close the "Terminal" application
6. Reopen the "Terminal" application
7. Type `rvm` and press `<Enter>`

### Check Your Work

If you see a long message ending in "For additional documentation please visit
https://rvm.io", continue below.

## Install Ruby version 2.6.1 on Ubuntu

For our Ruby labs and lessons, we expect that students use Ruby version 2.6.1.
If Ruby Environment Manager (RVM) has been successfully installed, you can
quickly install Ruby with a couple of commands.

### Action Item

1. Open the "Terminal" application using "Spotlight Search"
2. Type `rvm install 2.6.1` and press `<Enter>`
3. Type `rvm list` and press `<Enter>`

### Check Your Work

If you see a message starting with "=\* ruby-2.6.1", continue below.

## Install Ruby Gems

Ruby Gems are small programs written in Ruby that help you to code more easily
in Ruby. The gems you will install today include: Bundler, which allows you to
keep track of which gems your projects need to work; Pry, which allows you to
pause your code when it runs and inspect it; Nokogiri, which allows you to read
and pick apart HTML pages; and Ruby on Rails, which allows you to easily create
a web application with Ruby.

### Action Item

1. Open the "Terminal" application using "Spotlight Search"
2. Type `gem update --system` and press `<Enter>`
3. Type `gem install bundler` and press `<Enter>`
4. Type `gem install pry` and press `<Enter>`
5. Type `gem install nokogiri` and press `<Enter>` _(Note: this gem typically
   takes longer than the others to install)_
6. Type `gem install rails` and press `<Enter>`
7. Type `gem install learn-co` and press `<Enter>`
8. Type `gem list | wc -l` and press `<Enter>`

### Check Your Work

If you are able to complete each step without any issues, and you see an output
of a number around 100 from the last command, continue to the next lesson,
**Installing Node.js on macOS**.