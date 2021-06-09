# pysimplecache - Defines a simple cache of objects

pysimplecache implements a static class (`Cache`) to store (in a non-persistent way) and share objects of any type.

## Install
### From Conda
```sh
[sudo] conda install -c conda-forge -c pysimplecache
```

## Use
### Compound
```python
from pysimplecache import Cache

o = <any object>

Cache.add(obj=o, id='my_o')

oo = Cache.get('my_o')
```
This code creates an object of any type (int, List, Dict, custom object), dd it to the cache and read it from the cache.


## Tests
Please follow instructions below to run tests:
```
cd tests
pytest -v
```
For further tests and development tools, a CI toolkit is provided in `ci` folder (see [ci/README.md](ci/README.md)).


## Authors

* **Joan Hérisson**


## Licence
pysimplecache is released under the MIT licence. See the LICENCE file for details.
