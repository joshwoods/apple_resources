

- Core Foundation
-  CFBinaryHeap 

Class

# CFBinaryHeap

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CFBinaryHeap
```

## Overview

`CFBinaryHeap` implements a container that stores values sorted using a binary search algorithm. All binary heaps are mutable; there is not a separate immutable variety. Binary heaps can be useful as priority queues.

## Topics

### CFBinaryHeap Miscellaneous Functions

func CFBinaryHeapAddValue(CFBinaryHeap!, UnsafeRawPointer!)

Adds a value to a binary heap.

func CFBinaryHeapApplyFunction(CFBinaryHeap!, ((UnsafeRawPointer?, UnsafeMutableRawPointer?) -> Void)!, UnsafeMutableRawPointer!)

Iteratively applies a function to all the values in a binary heap.

func CFBinaryHeapContainsValue(CFBinaryHeap!, UnsafeRawPointer!) -> Bool

Returns whether a given value is in a binary heap.

func CFBinaryHeapCreate(CFAllocator!, CFIndex, UnsafePointer&lt;CFBinaryHeapCallBacks>!, UnsafePointer&lt;CFBinaryHeapCompareContext>!) -> CFBinaryHeap!

Creates a new mutable or fixed-mutable binary heap.

func CFBinaryHeapCreateCopy(CFAllocator!, CFIndex, CFBinaryHeap!) -> CFBinaryHeap!

Creates a new mutable or fixed-mutable binary heap with the values from a pre-existing binary heap.

func CFBinaryHeapGetCount(CFBinaryHeap!) -> CFIndex

Returns the number of values currently in a binary heap.

func CFBinaryHeapGetCountOfValue(CFBinaryHeap!, UnsafeRawPointer!) -> CFIndex

Counts the number of times a given value occurs in a binary heap.

func CFBinaryHeapGetMinimum(CFBinaryHeap!) -> UnsafeRawPointer!

Returns the minimum value in a binary heap.

func CFBinaryHeapGetMinimumIfPresent(CFBinaryHeap!, UnsafeMutablePointer&lt;UnsafeRawPointer?>!) -> Bool

Returns the minimum value in a binary heap, if present.

func CFBinaryHeapGetTypeID() -> CFTypeID

Returns the type identifier of the `CFBinaryHeap` opaque type.

func CFBinaryHeapGetValues(CFBinaryHeap!, UnsafeMutablePointer&lt;UnsafeRawPointer?>!)

Copies all the values from a binary heap into a sorted C array.

func CFBinaryHeapRemoveAllValues(CFBinaryHeap!)

Removes all values from a binary heap, making it empty.

func CFBinaryHeapRemoveMinimumValue(CFBinaryHeap!)

Removes the minimum value from a binary heap.

### Callbacks

typealias CFBinaryHeapApplierFunction

Callback function used to apply a function to all members of a binary heap.

var compare: ((UnsafeRawPointer?, UnsafeRawPointer?, UnsafeMutableRawPointer?) -> CFComparisonResult)!

The callback used to compare values in the binary heap in some operations. This field cannot be `NULL`.

var copyDescription: ((UnsafeRawPointer?) -> Unmanaged&lt;CFString>?)!

Callback function used to get a description of a value in a binary heap.

var release: ((CFAllocator?, UnsafeRawPointer?) -> Void)!

Callback function used to release a value before it is removed from a binary heap.

var retain: ((CFAllocator?, UnsafeRawPointer?) -> UnsafeRawPointer?)!

Callback function used to retain a value being added to a binary heap.

var version: CFIndex

The version number of the structure type being passed in as a parameter to the `CFBinaryHeap` creation functions. This structure is version `0`.

### Data Types

struct CFBinaryHeapCallBacks

Structure containing the callbacks for values for a `CFBinaryHeap` object.

struct CFBinaryHeapCompareContext

Not used.

### Constants

Predefined Callback Structures

`CFBinaryHeap` provides some predefined callbacks for your convenience.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Related Documentation

Collections Programming Topics

### Opaque Types

class CFAllocator

class CFArray

class CFAttributedString

class CFBag

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

class CFFileDescriptor

