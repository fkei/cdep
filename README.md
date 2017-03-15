# cdep
Classic Go dependency tool

Move the specified directory to one GOPATH.
Vendor function is not used.

It is very simple. Look at the example project.

Example: [https://github.com/fkei/stgoart](https://github.com/fkei/stgoart)

# install

Currnet install directory.

```
$ bash <(curl -s https://raw.githubusercontent.com/fkei/cdep/develop/install) `pwd`
```

Select(/xxxx/yyyy) install directory.

```
$ bash <(curl -s https://raw.githubusercontent.com/fkei/cdep/develop/install) /xxxx/yyyy
```

# Setup

Edit configure file. `cdep.conf`

Example file: [https://github.com/fkei/stgoart/blob/master/cdep.conf](https://github.com/fkei/stgoart/blob/master/cdep.conf)
```
# scm service domain. github.com, gitlab.com, bitbucket.org, golang.org, gopkg.in ...
SERVICE="XXXXXXXXXX"

# scm service organization name.
ORGANIZATION="YYYYYYYYYY"

# scm repository name
REPOSITORY="ZZZZZZZZZZ"
```

Edit dependency package list file. `cdep.lock`

Example file: [https://github.com/fkei/stgoart/blob/master/cdep.lock](https://github.com/fkei/stgoart/blob/master/cdep.lock)

# Use

Install and Update

```
$ ./cdep install
```

Uninstall

```
$ ./cdep uninstall
```

Help

```
$ ./cdep help
```
