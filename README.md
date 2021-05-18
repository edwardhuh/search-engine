# search-engine

My version of Bart de Goede's [search engine](https://bart.degoe.de/building-a-full-text-search-engine-150-lines-of-code/)

Some additional modifications and personalizations, but most of the credit should still go to Bart. 

Notes: 
* dataclass: simple data structures simply use tuple or a dict. 
However, there are many quality of life concerns, like indexing, that prevent easy access to elements.
A better alternative is the `namedtuple`.
```
from collections import namedtuple

NamedTupleCard = namedtuple('NamedTupleCard', ['rank', 'suit'])
```
Unfortunately, a namedtuple is by nature immutable. 
