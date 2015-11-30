
```
sudo -E apt-get install -y build-essential g++ git bison pkg-config re2c libxml2-dev libssl-dev libcurl4-openssl-dev libjpeg-dev libpng12-dev libmcrypt-dev libtidy-dev libreadline-dev libxslt1-dev libcurl4-openssl-dev libldap2-dev
mkdir -p ~/tools ; cd tools
git clone https://github.com/CHH/phpenv.git
cd phpenv
bash bin/phpenv-install.sh
echo 'export PATH=$HOME/.phpenv/bin:$PATH' >> $HOME/.bashrc
echo 'eval "$(phpenv init -)"' >> $HOME/.bashrc
cd $HOME/.phpenv/
git clone -b phpcc https://github.com/0livier/php-build.git plugins/php-build
cd plugins/php-build
sudo ln -fs /usr/lib/x86_64-linux-gnu/libldap.so /usr/lib/

```

