This website theme is based on [Caly53](https://github.com/clayh53/tufte-jekyll/tree/master) jekyll enhancements of the original [tufte-css](https://github.com/edwardtufte/tufte-css), and slightly modified. 

## Demo
You can find an Github Pages implemention [here](https://matthiasfrenzl.com)

# Preparation
## Get the repo
1) Either fork/clone or create a new empty Github repository
2) Copy this (master-branch) repository and put it in your local machine's github directory 
3) Commite it to Github
## Install the required software at your local machine in your local repository directory
```
homebrew
brew install chruby ruby-install xz
ruby-install ruby
gem install jekyll
gem install jekyll bundler
jekyll build 
bundle config set --local path vendor/bundle
bundle install
bundle add webrick
```
Check the versions with 
`jekyll -v`
`ruby -v`

## Run the server on your local machine
```
bundle exec jekyll serve
```
Check your website via your favorite browser at `http://127.0.0.1:4000`

Abort the local server with `CTRL` `C`

Kill the processes (if necessary) by first checking their PID with `lsof -wni tcp:4000` and then `kill -9 PID-Number`


## Deployment of the website at Github Pages
```
rake rakefile publish
rake -f UploadToGithub.Rakefile publish
```

## Upload a new blog post
1) Create an .md file and save it in the master-branch draft folder
```
rake 
```




