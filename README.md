[![](https://i.imgur.com/zNBkzj1.png)](https://beautifuljekyll.com/plans/)

# Beautiful Jekyll
[![Gem Version](https://badge.fury.io/rb/beautiful-jekyll-theme.svg)](https://badge.fury.io/rb/beautiful-jekyll-theme)


> By [Dean Attali](https://deanattali.com) &middot; [Demo](https://beautifuljekyll.com/)

**Beautiful Jekyll** is a ready-to-use template to help you create a beautiful website quickly. Perfect for personal sites, blogs, or simple project websites.  [Check out a demo](https://beautifuljekyll.com) of what you'll get after just two minutes.  You can also look at [my personal website](https://deanattali.com) or [my consulting website](https://attalitech.com) to see it in use, or see [examples of websites](http://beautifuljekyll.com/examples) other people created using this theme.

## Run blog in local
1. Install rbenv
first remove ruby: sudo apt purge ruby

Then reinstall ruby using rbenv and ruby-build according to their docs:

cd $HOME
sudo apt update 
sudo apt install git-core curl zlib1g-dev build-essential libssl-dev libreadline-dev libyaml-dev libxml2-dev libxslt1-dev libcurl4-openssl-dev libffi-dev

git clone https://github.com/rbenv/rbenv.git ~/.rbenv
echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bashrc
echo 'eval "$(rbenv init -)"' >> ~/.bashrc
exec $SHELL

git clone https://github.com/rbenv/ruby-build.git ~/.rbenv/plugins/ruby-build
echo 'export PATH="$HOME/.rbenv/plugins/ruby-build/bin:$PATH"' >> ~/.bashrc
exec $SHELL

rbenv install 3.3.1
rbenv global 3.3.1
ruby -v

The last step is to install Bundler:

gem install bundler
rbenv rehash

Vào thư mục cài đặt blog chạy lệnh 

bundle install

Sau khi cài xong, chạy lệnh sau để run blog in local

```
bundle exec jekyll serve
```
