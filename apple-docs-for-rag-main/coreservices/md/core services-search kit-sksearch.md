

- Core Services
- Search Kit
-  SKSearch 

Class

# SKSearch

Defines an opaque data type representing an asynchronous search.

Mac Catalyst 13.0+macOS 10.4+

``` source
class SKSearch
```

## Overview

A search object is created when you call the SKSearchCreate(_:_:_:) function.

### Special Considerations

You cannot use CFMakeCollectable with SKSearch objects. In a garbage-collected environment, you must use CFRelease to dispose of an SKSearch object.

