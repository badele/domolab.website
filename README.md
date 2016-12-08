# domolab.website
domolab website

The website source for http://badele.github.io/domolab.website

```bash
mkvirtualenv --no-site-packages -p /usr/bin/python2.7 lektor
git clone https://github.com/lektor/lektor
cd lektor
make build-js
pip install --editable .
```

## Edit
```bash
workon lektor
cd domolab.website
lektor server -f webpack
```