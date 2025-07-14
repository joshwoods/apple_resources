

- Core Foundation
-  CFPlugInInstance 

Class

# CFPlugInInstance

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CFPlugInInstance
```

## Overview

CFPlugInInstance is deprecated. Use the functions defined by CFPlugIn instead.

## Topics

### Deprecated

func CFPlugInInstanceCreateWithInstanceDataSize(CFAllocator!, CFIndex, CFPlugInInstanceDeallocateInstanceDataFunction!, CFString!, CFPlugInInstanceGetInterfaceFunction!) -> CFPlugInInstance!

Not recommended.

func CFPlugInInstanceGetFactoryName(CFPlugInInstance!) -> CFString!

Not recommended.

func CFPlugInInstanceGetInstanceData(CFPlugInInstance!) -> UnsafeMutableRawPointer!

Not recommended.

func CFPlugInInstanceGetInterfaceFunctionTable(CFPlugInInstance!, CFString!, UnsafeMutablePointer&lt;UnsafeMutableRawPointer?>!) -> Bool

Not recommended.

func CFPlugInInstanceGetTypeID() -> CFTypeID

Not recommended.

### Callbacks

typealias CFPlugInInstanceDeallocateInstanceDataFunction

Not recommended.

typealias CFPlugInInstanceGetInterfaceFunction

Not recommended.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

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

