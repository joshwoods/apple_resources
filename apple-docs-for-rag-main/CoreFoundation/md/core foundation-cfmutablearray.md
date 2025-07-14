

- Core Foundation
-  CFMutableArray 

Class

# CFMutableArray

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CFMutableArray
```

## Overview

CFMutableArray manages dynamic arrays. The basic interface for managing arrays is provided by CFArray. CFMutableArray adds functions to modify the contents of an array.

You create a mutable array object using either the CFArrayCreateMutable(_:_:_:) or CFArrayCreateMutableCopy(_:_:_:) function.

CFMutableArray provides several functions for changing the contents of an array, for example the CFArrayAppendValue(_:_:) and CFArrayInsertValueAtIndex(_:_:_:) functions add values to an array and CFArrayRemoveValueAtIndex(_:_:) removes values from an array. You can also reorder the contents of an array using CFArrayExchangeValuesAtIndices(_:_:_:) and CFArraySortValues(_:_:_:_:).

CFMutableArray is “toll-free bridged” with its Cocoa Foundation counterpart, NSMutableArray. This means that the Core Foundation type is interchangeable in function or method calls with the bridged Foundation object. Therefore, in a method where you see an `NSMutableArray *` parameter, you can pass in a `CFMutableArrayRef`, and in a function where you see a `CFMutableArrayRef` parameter, you can pass in an NSMutableArray instance. This fact also applies to concrete subclasses of NSMutableArray. See Toll-Free Bridged Types for more information on toll-free bridging.

## Topics

### CFMutableArray Miscellaneous Functions

func CFArrayAppendArray(CFMutableArray!, CFArray!, CFRange)

Adds the values from one array to another array.

func CFArrayAppendValue(CFMutableArray!, UnsafeRawPointer!)

Adds a value to an array giving it the new largest index.

func CFArrayCreateMutable(CFAllocator!, CFIndex, UnsafePointer&lt;CFArrayCallBacks>!) -> CFMutableArray!

Creates a new empty mutable array.

func CFArrayCreateMutableCopy(CFAllocator!, CFIndex, CFArray!) -> CFMutableArray!

Creates a new mutable array with the values from another array.

func CFArrayExchangeValuesAtIndices(CFMutableArray!, CFIndex, CFIndex)

Exchanges the values at two indices of an array.

func CFArrayInsertValueAtIndex(CFMutableArray!, CFIndex, UnsafeRawPointer!)

Inserts a value into an array at a given index.

func CFArrayRemoveAllValues(CFMutableArray!)

Removes all the values from an array, making it empty.

func CFArrayRemoveValueAtIndex(CFMutableArray!, CFIndex)

Removes the value at a given index from an array.

func CFArrayReplaceValues(CFMutableArray!, CFRange, UnsafeMutablePointer&lt;UnsafeRawPointer?>!, CFIndex)

Replaces a range of values in an array.

func CFArraySetValueAtIndex(CFMutableArray!, CFIndex, UnsafeRawPointer!)

Changes the value at a given index in an array.

func CFArraySortValues(CFMutableArray!, CFRange, CFComparatorFunction!, UnsafeMutableRawPointer!)

Sorts the values in an array using a given comparison function.

## Relationships

### Inherits From

- CFArray

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

