# Build and publish mecab-ipadic-NEologd

[![Build Status](https://travis-ci.org/pypt/publish-mecab-ipadic-neologd-builds.svg?branch=develop)](https://travis-ci.org/pypt/publish-mecab-ipadic-neologd-builds)

This repository builds, tags and publishes unofficial [mecab-ipadic-NEologd](https://github.com/neologd/mecab-ipadic-neologd) builds to make them easier to install.


## Installing mecab-ipadic-NEologd


### Debian / Ubuntu

You can download pre-build mecab-ipadic-neologd `.deb` packages via APT:

```bash
# Add Bintray's GPG key
sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 379CE192D401AB61

# Add mecab-ipadic-neologd APT repository
echo "deb https://dl.bintray.com/neologd-unofficial/mecab-ipadic-neologd-deb stable main" | sudo tee -a /etc/apt/sources.list.d/mecab-ipadic-neologd.list

# Update APT package listing
sudo apt-get -y update

# Install mecab-ipadic-neologd
sudo apt-get -y install mecab-ipadic-neologd
```

or from our [GitHub releases](releases) page.

mecab-ipadic-NEologd data files will be available at `/var/lib/mecab/dic/ipadic-neologd`.


### Red Hat / CentOS

You can download pre-build mecab-ipadic-neologd `.rpm` packages via YUM:

```bash
# Add repository that provides mecab RPM
sudo yum install -y https://packages.groonga.org/centos/groonga-release-latest.noarch.rpm
sudo yum makecache

# Add mecab-ipadic-neologd YUM repository
sudo curl https://bintray.com/neologd-unofficial/mecab-ipadic-neologd-rpm/rpm -o /etc/yum.repos.d/mecab-ipadic-neologd.repo

# Install mecab-ipadic-neologd
sudo yum install -y mecab-ipadic-neologd
```

or from our [GitHub releases](releases) page.

mecab-ipadic-NEologd data files will be available at `/usr/lib64/mecab/dic/ipadic-neologd`.


### Tarball

You can download pre-build mecab-ipadic-NEologd tarball packages from:

**<https://bintray.com/neologd-unofficial/mecab-ipadic-neologd-tgz>**

or from our [GitHub releases](releases) page.
