

- Core Foundation
-  CFArray 

Class

# CFArray

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CFArray
```

## Overview

CFArray and its derived mutable type, CFMutableArray, manage ordered collections of values called arrays. CFArray creates static arrays and CFMutableArray creates dynamic arrays.

You create a static array object using either the CFArrayCreate(_:_:_:_:) or CFArrayCreateCopy(_:_:) function. These functions return an array containing the values you pass in as arguments. (Note that arrays can’t contain `NULL` pointers; in most cases, though, you can use the kCFNull constant instead.) Values are not copied but retained using the retain callback provided when an array was created. Similarly, when a value is removed from an array, it is released using the release callback.

CFArray’s two primitive functions CFArrayGetCount(_:) and CFArrayGetValueAtIndex(_:_:) provide the basis for all other functions in its interface. The CFArrayGetCount(_:) function returns the number of elements in an array; CFArrayGetValueAtIndex(_:_:) gives you access to an array’s elements by index, with index values starting at 0.

A number of CFArray functions allow you to operate over a range of values in an array, for example CFArrayApplyFunction(_:_:_:_:) lets you apply a function to values in an array, and CFArrayBSearchValues(_:_:_:_:_:) searches an array for the value that matches its parameter. Recall that a range is defined as `{start, length}`, therefore to operate over the entire array the range you supply should be `{0, N}` (where `N` is the count of the array).

CFArray is “toll-free bridged” with its Cocoa Foundation counterpart, NSArray. This means that the Core Foundation type is interchangeable in function or method calls with the bridged Foundation object. Therefore, in a method where you see an `NSArray *` parameter, you can pass in a `CFArrayRef`, and in a function where you see a `CFArrayRef` parameter, you can pass in an NSArray instance. This also applies to concrete subclasses of NSArray. See Toll-Free Bridged Types for more information on toll-free bridging.

## Topics

### Creating an Array

func CFArrayCreate(CFAllocator!, UnsafeMutablePointer&lt;UnsafeRawPointer?>!, CFIndex, UnsafePointer&lt;CFArrayCallBacks>!) -> CFArray!

Creates a new immutable array with the given values.

func CFArrayCreateCopy(CFAllocator!, CFArray!) -> CFArray!

Creates a new immutable array with the values from another array.

### Examining an Array

func CFArrayBSearchValues(CFArray!, CFRange, UnsafeRawPointer!, CFComparatorFunction!, UnsafeMutableRawPointer!) -> CFIndex

Searches an array for a value using a binary search algorithm.

func CFArrayContainsValue(CFArray!, CFRange, UnsafeRawPointer!) -> Bool

Reports whether or not a value is in an array.

func CFArrayGetCount(CFArray!) -> CFIndex

Returns the number of values currently in an array.

func CFArrayGetCountOfValue(CFArray!, CFRange, UnsafeRawPointer!) -> CFIndex

Counts the number of times a given value occurs in an array.

func CFArrayGetFirstIndexOfValue(CFArray!, CFRange, UnsafeRawPointer!) -> CFIndex

Searches an array forward for a value.

func CFArrayGetLastIndexOfValue(CFArray!, CFRange, UnsafeRawPointer!) -> CFIndex

Searches an array backward for a value.

func CFArrayGetValues(CFArray!, CFRange, UnsafeMutablePointer&lt;UnsafeRawPointer?>!)

Fills a buffer with values from an array.

func CFArrayGetValueAtIndex(CFArray!, CFIndex) -> UnsafeRawPointer!

Retrieves a value at a given index.

### Applying a Function to Elements

func CFArrayApplyFunction(CFArray!, CFRange, ((UnsafeRawPointer?, UnsafeMutableRawPointer?) -> Void)!, UnsafeMutableRawPointer!)

Calls a function once for each element in range in an array.

### Getting the CFArray Type ID

func CFArrayGetTypeID() -> CFTypeID

Returns the type identifier for the CFArray opaque type.

### Callbacks

typealias CFArrayApplierFunction

Prototype of a callback function that may be applied to every value in an array.

typealias CFArrayCopyDescriptionCallBack

Prototype of a callback function used to get a description of a value in an array.

typealias CFArrayEqualCallBack

Prototype of a callback function used to determine if two values in an array are equal.

typealias CFArrayReleaseCallBack

Prototype of a callback function used to release a value before it’s removed from an array.

typealias CFArrayRetainCallBack

Prototype of a callback function used to retain a value being added to an array.

### Data Types

struct CFArrayCallBacks

Structure containing the callbacks of a CFArray.

### Constants

Predefined Callback Structures

CFArray provides a predefined callback structure appropriate for use when the values in a CFArray are all CFType-derived objects.

## Relationships

### Inherited By

- CFMutableArray

### Conforms To

- Equatable
- Hashable

## See Also

### Related Documentation

Property List Programming Topics for Core Foundation

Collections Programming Topics for Core Foundation

### Opaque Types

class CFAllocator

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

class CFFileDescriptor

