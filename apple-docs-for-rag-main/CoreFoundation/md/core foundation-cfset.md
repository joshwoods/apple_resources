

- Core Foundation
-  CFSet 

Class

# CFSet

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CFSet
```

## Overview

CFSet and its derived mutable type, CFMutableSet, provide support for the mathematical concept of a set. A set, both in its mathematical sense and in the implementation of CFSet, is an unordered collection of distinct elements. CFSet creates static sets and CFMutableSet creates dynamic sets.

Use bags or sets as an alternative to arrays when the order of elements isn’t important and performance in testing whether a value is contained in the collection is a consideration—while arrays are ordered, testing for membership is slower than with bags or sets. Use bags over sets if you want to allow duplicate values in your collections.

You create a static set object using either the CFSetCreate(_:_:_:_:) or CFSetCreateCopy(_:_:) function. These functions return a set containing the values you pass in as arguments. (Note that sets can’t contain `NULL` pointers; in most cases, though, you can use the kCFNull constant instead.) Values are not copied but retained using the retain callback provided when the set was created. Similarly, when a value is removed from a set, it is released using the release callback.

CFSet provides functions for querying the values of a set. The CFSetGetCount(_:) returns the number of values in a set, the CFSetContainsValue(_:_:) function checks if a value is in a set, and CFSetGetValues(_:_:) returns a C array containing all the values in a set.

CFSet is “toll-free bridged” with its Cocoa Foundation counterpart, NSSet. This means that the Core Foundation type is interchangeable in function or method calls with the bridged Foundation object. Therefore, in a method where you see an `NSSet *` parameter, you can pass in a `CFSetRef`, and in a function where you see a `CFSetRef` parameter, you can pass in an NSSet instance. This also applies to concrete subclasses of NSSet. See Toll-Free Bridged Types for more information on toll-free bridging.

## Topics

### Creating Sets

func CFSetCreate(CFAllocator!, UnsafeMutablePointer&lt;UnsafeRawPointer?>!, CFIndex, UnsafePointer&lt;CFSetCallBacks>!) -> CFSet!

Creates an immutable CFSet object containing supplied values.

func CFSetCreateCopy(CFAllocator!, CFSet!) -> CFSet!

Creates an immutable set containing the values of an existing set.

### Examining a Set

func CFSetContainsValue(CFSet!, UnsafeRawPointer!) -> Bool

Returns a Boolean that indicates whether a set contains a given value.

func CFSetGetCount(CFSet!) -> CFIndex

Returns the number of values currently in a set.

func CFSetGetCountOfValue(CFSet!, UnsafeRawPointer!) -> CFIndex

Returns the number of values in a set that match a given value.

func CFSetGetValue(CFSet!, UnsafeRawPointer!) -> UnsafeRawPointer!

Obtains a specified value from a set.

func CFSetGetValueIfPresent(CFSet!, UnsafeRawPointer!, UnsafeMutablePointer&lt;UnsafeRawPointer?>!) -> Bool

Reports whether or not a value is in a set, and if it exists returns the value indirectly.

func CFSetGetValues(CFSet!, UnsafeMutablePointer&lt;UnsafeRawPointer?>!)

Obtains all values in a set.

### Applying a Function to Set Members

func CFSetApplyFunction(CFSet!, ((UnsafeRawPointer?, UnsafeMutableRawPointer?) -> Void)!, UnsafeMutableRawPointer!)

Calls a function once for each value in a set.

### Getting the CFSet Type ID

func CFSetGetTypeID() -> CFTypeID

Returns the type identifier for the CFSet type.

### Callbacks

typealias CFSetApplierFunction

Prototype of a callback function that may be applied to every value in a set.

typealias CFSetCopyDescriptionCallBack

Prototype of a callback function used to get a description of a value in a set.

typealias CFSetEqualCallBack

Prototype of a callback function used to determine if two values in a set are equal.

typealias CFSetHashCallBack

Prototype of a callback function called to compute a hash code for a value. Hash codes are used when values are accessed, added, or removed from a collection.

typealias CFSetReleaseCallBack

Prototype of a callback function used to release a value before it’s removed from a set.

typealias CFSetRetainCallBack

Prototype of a callback function used to retain a value being added to a set.

### Data Types

struct CFSetCallBacks

This structure contains the callbacks used to retain, release, describe, and compare the values of a CFSet object.

### Constants

Predefined Callback Structures

CFSet provides some predefined callbacks for your convenience.

## Relationships

### Inherited By

- CFMutableSet

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

