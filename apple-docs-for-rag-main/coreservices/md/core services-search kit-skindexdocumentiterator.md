

- Core Services
- Search Kit
-  SKIndexDocumentIterator 

Class

# SKIndexDocumentIterator

Defines an opaque data type representing an index-based document iterator.

Mac Catalyst 13.0+macOS 10.3+

``` source
class SKIndexDocumentIterator
```

## Overview

A Search Kit document iterator lets your application loop through all the document URL objects owned by a given parent document URL object. To create an iterator, use SKIndexDocumentIteratorCreate(_:_:). To get a copy of the next document in the set owned by the iterator, use SKIndexDocumentIteratorCopyNext(_:).

