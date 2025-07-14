

- Core Foundation
-  CFMutableBag 

Class

# CFMutableBag

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CFMutableBag
```

## Overview

CFMutableBag manages dynamic bags. The basic interface for managing bags is provided by CFBag. CFMutableBag adds functions to modify the contents of a bag.

You create a mutable bag object using either the CFBagCreateMutable(_:_:_:) or CFBagCreateMutableCopy(_:_:_:) function.

CFMutableBag provides several functions for adding and removing values from a bag. The CFBagAddValue(_:_:) function adds a value to a bag and CFBagRemoveValue(_:_:) removes values from a bag.

## Topics

### Creating a Mutable Bag

func CFBagCreateMutable(CFAllocator!, CFIndex, UnsafePointer&lt;CFBagCallBacks>!) -> CFMutableBag!

Creates a new empty mutable bag.

func CFBagCreateMutableCopy(CFAllocator!, CFIndex, CFBag!) -> CFMutableBag!

Creates a new mutable bag with the values from another bag.

### Modifying a Mutable Bag

func CFBagAddValue(CFMutableBag!, UnsafeRawPointer!)

Adds a value to a mutable bag.

func CFBagRemoveAllValues(CFMutableBag!)

Removes all values from a mutable bag.

func CFBagRemoveValue(CFMutableBag!, UnsafeRawPointer!)

Removes a value from a mutable bag.

func CFBagReplaceValue(CFMutableBag!, UnsafeRawPointer!)

Replaces a value in a mutable bag.

func CFBagSetValue(CFMutableBag!, UnsafeRawPointer!)

Sets a value in a mutable bag.

## Relationships

### Inherits From

- CFBag

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

