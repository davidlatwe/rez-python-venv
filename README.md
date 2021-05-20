# Virtual env based python rez package

This is a *combined* package, which cannot be built but simply copying `python.py` into package repository.
And it will provide clean, re-usable virtual env that created from system installed python that it could find.
```
$ rez-search python
python-2.7-venv
python-3.6-venv
python-3.7-venv
python-3.8-venv
```

### requirement
These (pip) packages should be installed in Rez production env:
* [pythonfinder](https://github.com/sarugaku/pythonfinder)
* [virtualenv](https://github.com/pypa/virtualenv)


### Caveat

If regular `python` package (dir) and `python.py` combined pacakge both exists in same filesystem repository, only dir package will be iterated, so you have to place the combined one in another repository. e.g. `~/rez/package/combined`

