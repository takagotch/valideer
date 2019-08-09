### valideer
---
https://github.com/podio/valideer

```py
// valideer/tests/test_validators.py
from datetime import date, datetime
from decimal import Decimal
from functools import partial, wraps
import collections
import json
import re
import unittest
import valideer as V
from valideer.compact import long, unicode, xrange, string_types, int_types

class Fraction(V.Type):
  name = "fraction"
  accept_type = (float, complex, Decimal)

class Date(V.Type):
  accept_types = (date, datetime)
  
class Gender(V.Enum):
  name = "gender"
  values = {"male", "female", "it's complicated"}

class TestValidator(unittest.TestCase):
  parse = staticmethod(V.parse)
  
  def setup(self):
    V.Object.REQUIRED_PROPERTIES = True
      V.Object.REQUIRED_PROPERTIES = True
      V.base.reset_type_names()
      self.complex_validator = self.parse({
        "n": "number",
        "?i": V.Numable("integer", 0),
      })


```

```
```

```
```


