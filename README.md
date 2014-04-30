
![Build Status] (https://secure.travis-ci.org/vmalloc/hooky.png )


![Downloads] (https://pypip.in/d/hooky/badge.png )

![Version] (https://pypip.in/v/hooky/badge.png )

# Overview

`hooky` is a library implementing a basic hook mechanism for implementing callbacks. It provides flexible configuration, hook namespaces and error handling strategies.

# Installation

```
$ pip install hooky
```

# Usage

The simplest use case when we want to register a callback to be called later. We start by registering a callback through `hooky.register`:

```python

>>> from __future__ import print_function
>>> import hooky
>>> @hooky.register('hook_name')
... def func():
...     print('Called')

```

Now we can call the hook:

```python

>>> hooky.trigger('hook_name')
Called

```

For more advanced uses, please refer to [the documentation](http://hooky.readthedocs.org ) 
										

# Licence

BSD3

