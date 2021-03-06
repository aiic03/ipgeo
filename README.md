ipgeo
===========
[![Build Status](https://travis-ci.org/aiic03/ipgeo.svg?branch=master)](https://travis-ci.org/aiic03/ipgeo)[![PyPI version](https://badge.fury.io/py/ipgeo.svg)](http://badge.fury.io/py/ipgeo)[![Coverage Status](https://coveralls.io/repos/aiic03/ipgeo/badge.svg)](https://coveralls.io/r/aiic03/ipgeo)[![Code Health](https://landscape.io/github/aiic03/ipgeo/master/landscape.svg?style=flat)](https://landscape.io/github/aiic03/ipgeo/master)
[![Stories in Ready](https://badge.waffle.io/aiic03/ipgeo.svg?label=ready&title=Ready)](http://waffle.io/aiic03/ipgeo)


Geo info retriver for ipv4 address using chinese taobao service.

Python 2.x/3.x Compatible.

Inspired by [huacnlee/ip-location](https://github.com/huacnlee/ip-location).

## Goal

Retrieve geo info for ip address via [ip.taobao.com](http://ip.taobao.com) .

## Limit

* The official limit: for every user, qps < 10. [ref](http://ip.taobao.com/restrictions.php)

## Usage

```python
#encoding=utf8

from ipgeo import ipgeo

info = ipgeo.query('182.138.127.93')
print(info.country)      # 中国
print(info.region)       # 四川省
print(info.city)         # 成都市
print(info.full_name())  # 中国四川省成都市
```
