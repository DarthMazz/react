# node install

## refernece

https://blog.mintsu-dev.com/posts/2020-07-22-install-nodenv-linux/


## install commands

on Windows 11 in WSL

1. Clone nodenv
```
git clone https://github.com/nodenv/nodenv.git ~/.nodenv
```

2. nodenv in PATH

```
echo 'export PATH="$HOME/.nodenv/bin:$PATH"' >> ~/.bashrc
```

3. nodenv init at login
```
echo 'eval "$(nodenv init -)"' >> ~/.bashrc
```

4. reload bashrc
```
source ~/.bashrc
```

5. add install command
```
git clone https://github.com/nodenv/node-build.git $(nodenv root)/plugins/node-build
```

6. evaluate node
```
curl -fsSL https://github.com/nodenv/nodenv-installer/raw/master/bin/nodenv-doctor | bash
``` 

## install node

1. show list node versions
```
nodenv install -l
```

2. install node version
```
nodenv install 16.4.2
```

3. set node global setting
```
node global 16..4.2
```
