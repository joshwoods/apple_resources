

- Core Foundation
-  CFNull 

Class

# CFNull

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CFNull
```

## Overview

The CFNull opaque type defines a unique object used to represent null values in collection objects (which don’t allow `NULL` values). CFNull objects are neither created nor destroyed. Instead, a single CFNull constant object—kCFNull—is defined and is used wherever a null value is needed.

The CFNull opaque type is available in macOS 10.2 and later.

## Topics

### CFNull Miscellaneous Functions

func CFNullGetTypeID() -> CFTypeID

Returns the type identifier for the CFNull opaque type.

### Constants

Predefined Value

Predefined CFNull object.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Related Documentation

Collections Programming Topics for Core Foundation

### Opaque Types

class CFAllocator

class CFArray

class CFAttributedString

class CFBag

class CFBinaryHeap

class CFBitVector

class CFBoolean

class CFBundle

class CFCalendar

class CFCharacterSet

class CFData

class CFDate

class CFDateFormatter

class CFDictionary

class CFError

