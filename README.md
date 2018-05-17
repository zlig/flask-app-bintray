# flask-app-bintray [![Build Status](https://travis-ci.org/zlig/flask-app-bintray.svg?branch=master)](https://travis-ci.org/zlig/flask-app-bintray)  [ ![Download](https://api.bintray.com/packages/zlig/debian/flask-app-bintray/images/download.svg) ](https://bintray.com/zlig/debian/flask-app-bintray#files)

## Description

Build a Python Flask web application in a Debian .deb package using Travis and upload to Bintray 


## Usage

* Install the repository information and associated GPG key (to ensure authenticity):
```
$ echo "deb https://dl.bintray.com/zlig/debian /" | sudo tee -a /etc/apt/sources.list.d/zlig.list
$ sudo apt-key adv --recv-keys --keyserver keyserver.ubuntu.com EA3E6BAEB37CF5E4
```

* Update repository list of available packages and clean already installed versions
```
$ sudo apt update
$ sudo apt clean
```

* Reload services and start ours
```
$ sudo systemctl daemon-reload
$ sudo systemctl start flask-app-bintray
$ sudo systemctl status flask-app-bintray
```
