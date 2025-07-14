

- Core Foundation
-  CFBoolean 

Class

# CFBoolean

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CFBoolean
```

## Overview

CFBoolean objects are used to wrap boolean values for use in Core Foundation property lists and collection types.

## Topics

### CFBoolean Miscellaneous Functions

func CFBooleanGetTypeID() -> CFTypeID

Returns the Core Foundation type identifier for the CFBoolean opaque type.

func CFBooleanGetValue(CFBoolean!) -> Bool

Returns the value of a CFBoolean object as a standard C type `Boolean`.

### Constants

Boolean Values

CFBoolean evaluates to either true or false values where `kCFBooleanTrue` is the true, and `kCFBooleanFalse` is the false value.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Related Documentation

Property List Programming Topics for Core Foundation

### Opaque Types

class CFAllocator

class CFArray

class CFAttributedString

class CFBag

class CFBinaryHeap

class CFBitVector

class CFBundle

class CFCalendar

class CFCharacterSet

class CFData

class CFDate

class CFDateFormatter

class CFDictionary

class CFError

class CFFileDescriptor

