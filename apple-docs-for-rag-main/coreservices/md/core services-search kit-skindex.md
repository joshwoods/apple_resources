

- Core Services
- Search Kit
-  SKIndex 

Class

# SKIndex

Defines an opaque data type representing an index.

Mac Catalyst 13.0+macOS 10.3+

``` source
class SKIndex
```

## Overview

A Search Kit index object contains the textual contents of one or more documents, as well as document URL objects (SKDocumentRefs) representing those documents’ locations.

To create a new disk-based Search Kit index object, use SKIndexCreateWithURL(_:_:_:_:). To create a memory-based index, use SKIndexCreateWithMutableData(_:_:_:_:). For other operations on indexes, see Creating, Opening, and Closing Indexes and Managing Indexes. Also seeFast Asynchronous Searching.

### Special Considerations

You cannot use CFMakeCollectable with SKIndex objects. In a garbage-collected environment, you must use SKIndexClose(_:) to dispose of an SKIndex object.

