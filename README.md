# jo

![jo logo](jo-logo.png)

This is `jo`, a small utility to create JSON objects

```bash
$ jo -p name=jo n=17 parser@0
{
    "name": "jo",
    "n": 17,
    "parser": false
}
```

or arrays

```bash
$ seq 1 10 | jo -a
[1,2,3,4,5,6,7,8,9,10]
```

It has a [manual](jo.md), and you can read [why I wrote jo](http://jpmens.net/2016/03/05/a-shell-command-to-create-json-jo/).

## Build from Github

To install from the repository, you will need a C compiler as well as a relatively recent version of _automake_ and _autoconf_.

```bash
git clone git://github.com/jpmens/jo.git
cd jo
autoreconf -i
./configure
make check
make install
```


## Build from Release tarball

To build from [a release](https://github.com/jpmens/jo/releases) you will need a C compiler to install from a source tarball.

```bash
tar xvzf jo-0.?.tar.gz
cd jo-0.?
./configure
make check
make install
```
