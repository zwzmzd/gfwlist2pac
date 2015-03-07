GFWList2PAC
===========

[![PyPI version]][PyPI] [![Build Status]][Travis CI] 

Generate O(1) PAC file from gfwlist.

### Usage

	python main.py -f a.pac -p "SOCKS5 127.0.0.1:1080" --user-rule custom.txt --via-proxy "SOCKS5 127.0.0.1:1080"

### Performance

An example of generated PAC file is [here][example].

The PAC generated by GFWList2PAC is 1700x faster than SwitchySharp.

    Testing pac generated by gfwlist2pac
    total: 35.115832999999995ms
    avg: 0.5074542341040461ns

    Testing pac generated by switchysharp
    total: 58800.679729ms
    avg: 849.72080533237ns

[Build Status]: https://img.shields.io/travis/clowwindy/gfwlist2pac/master.svg?style=flat
[Travis CI]:    https://travis-ci.org/clowwindy/gfwlist2pac
[PyPI]:         https://pypi.python.org/pypi/gfwlist2pac
[PyPI version]: https://img.shields.io/pypi/v/gfwlist2pac.svg?style=flat
[example]:      https://github.com/clowwindy/gfwlist2pac/blob/master/test/proxy.pac
