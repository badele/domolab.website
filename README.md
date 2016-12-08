# domolab.website
domolab website

The website source for http://badele.github.io/domolab.website

```bash
git clone https://github.com/lektor/lektor
git clone https://github.com/badele/domolab.website
cd lektor
git reset --hard aa4e8cc5409532032f278edf35afd23a0f8cdd5a
make build-js
virtualenv --no-site-packages -p /usr/bin/python2.7 venv
. venv/bin/activate
pip install --editable .
pip install --upgrade setuptools
```

## Edit
```bash
cd lektor
. venv/bin/activate
cd domolab.website
lektor server -f webpack
curl localhost:5000
```

## Commit & Deploy
```
git commit -a -m "Update doc"
git push origin
lektor deploy ghpages
```
