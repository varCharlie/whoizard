# WHOIZARD
`whoizard` is a program for checking whether or not domains are registered. It can read domains over stdin, from a file, or from a space seperated list provided as an option.

I made `whoizard` because manually checking if domain names are registered can be tedious. The output of whoizard is each domain names expiration date, or a string letting you know the domain doesn't exist yet.


## Here is a simple interactive mode:

```bash
❯❯ whoizard
charlie.io
charlie.io: Registry Expiry Date: 2019-07-17T00:10:09Z
charles.com
charles.com:    Registry Expiry Date: 2018-05-17T04:00:00Z
^D
```


## Here is a simple file input mode:
```bash
❯❯ whoizard -f data/numbers/leading-zero-net -s 1 -C 4
0000.net:    Registry Expiry Date: 2019-01-01T11:59:59Z
0001.net:    Registry Expiry Date: 2018-04-17T18:29:28Z
0002.net:    Registry Expiry Date: 2018-10-14T01:38:56Z
0003.net:    Registry Expiry Date: 2019-01-08T00:20:05Z
0004.net:    Registry Expiry Date: 2018-12-08T19:10:03Z
0005.net:    Registry Expiry Date: 2018-09-05T18:14:24Z
0006.net:    Registry Expiry Date: 2020-02-11T19:05:32Z
0007.net:    Registry Expiry Date: 2020-10-28T19:07:39Z
```
