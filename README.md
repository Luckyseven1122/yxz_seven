# Some issues occurs when running this file locally based on localhost:4000

## Relationship between Ruby, Gem and Bundler
* Ruby is OOB (object oriented) programming language for website building
* Gem is Ruby language's package mamagement system; Ruby is like Python; Gem is like pip
* Bundler is command code for version control of Ruby
* Gemfile is like requirements.text or requirements.yml in python, in which all ruby packages used for this project is written, it can be compile 
* Based on compiled Gemfile, the bundler will automatically generate Gemfile.lock

## Installation steps
1. Install ruby (No issue): 
2. Install node (No issue): 
3. Install bundler (error: version of ruby is not compatible): 
    how to install the ruby with specific version using rbenv:
    - brew update
    - brew install rbenv ruby-build
    * initialize rbenv
        - echo 'eval "$(rbenv init -)"' >> ~/.zshrc
        - source ~/.zshrc
    * show available ruby version 
        - rbenv install -l
    - rbenv install 3.3.6
    * make system use newest version of ruby 
        - rbenv global 3.3.6
    * show current version that system recognize 
        - ruby -v
    - gem install bundler 
    - gem install jekyll bundler
    - bundle install
    - enter cv folder path: cd /Users/yaoxuanzhu/Documents/Github_personal_web/Yaoxuan_Seven.github.io
    - jekyll serve -l -H localhost -P 4001 
        * encouter issue: 
        "You have already activated public_suffix 6.0.1, but your Gemfile requires public_suffix 5.1.1. Prepending `bundle exec` to your command may solve this. (Gem::LoadError)"
        * Solution: change code
        - bundle exec jekyll serve -l -H localhost
    * jump out of command 
        - ctrl + c

## PS: 
- The external website: https://luckyseven1122.github.io/yxz_seven (related repo in Github needs to be published, otherwise, website will not display the content)
