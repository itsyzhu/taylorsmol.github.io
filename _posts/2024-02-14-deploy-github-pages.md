---
layout: post
title:  "Deploy GitHub Pages"
---

Create a new respositories on GitHub and clone it to your $HOME

---

Go to your blog folder
``` bash
cd YOUR-RESPOSITORIES
mkdir blog
```

---

Install requirements `Ruby`
``` bash
brew install rbenv

# list latest stable versions:
rbenv install -l

# install a Ruby version:
rbenv install 3.3.0

# view or change the global Ruby version
rbenv global 3.3.0

# view or change the Ruby version for the current shell session
rbenv local 3.3.0

# regenerate shims for all known Ruby executables
rbenv rehash

# help bootstrap rbenv into the current shell environment
rbenv init

# check your path (.zprofile)
export PATH="$HOME/.rbenv/versions/3.3.0/bin:$PATH"

# check the Ruby version you are using
which ruby
```

---

Use jekyll to initialize
``` bash
gem install jekyll

jekyll new .

bundler

bundle exec jekyll serve # Server address: http://127.0.0.1:4000/
```
