## Installation Instructions

0. Install [GitHub for Windows](http://desktop.github.com)
1. [Install Ruby 2.2 (not x64)](http://rubyinstaller.org)
  * Install folder should be `c:\Ruby22`
  * Check **Add Ruby executables to your PATH**, leave other options unchecked.
2. Install the appropriate DevKit
  * Install folder should be `c:\RubyDevKit`
3. Run **Git Shell**
4. Go to the DevKit folder `cd \RubyDevKit`
5. Run `ruby dk.rb init`
6. Run `cat config.yml`, you should see the line: `- C:/Ruby22`
7. Run `ruby dk.rb install`
8. Check versions:
  * `ruby -v` should show something like `ruby 2.2...`
  * `sqlite3 --version` should show something like: `3.8....`, if not:
    1. [Download precompiled shell version for windows](https://www.sqlite.org/download.html)
    2. Create folder `c:\sqlite`
    3. Unzip downloaded .exe to folder
    4. Add `c:\sqlite` to the `PATH` environment variable
9. `gem install rails`
  * You may get something saying the firewall has blocked the Ruby Interpreter, if so, allow it on both public and private networks
10. `rails -v` should show something like `Rails 4.2...`

[Rails Getting Started Guide](http://guides.rubyonrails.org/getting_started.html)

