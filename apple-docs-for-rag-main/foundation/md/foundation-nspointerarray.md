

- Foundation
-  NSPointerArray 

Class

# NSPointerArray

A collection similar to an array, but with a broader range of available memory semantics.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSPointerArray
```

## Overview

The pointer array class is modeled after NSArray, but can also hold `nil` values. You can insert or remove `nil` values which contribute to the array’s count.

A pointer array can be initialized to maintain strong or weak references to objects, or according to any of the memory or personality options defined by NSPointerFunctions.Options.

The NSCopying and NSCoding protocols are applicable only when a pointer array is initialized to maintain strong or weak references to objects.

When enumerating a pointer array with NSFastEnumeration using `for...in`, the loop will yield any `nil` values present in the array. See Fast Enumeration Makes It Easy to Enumerate a Collection in Programming with Objective-C for more information.

### Subclassing Notes

`NSPointerArray` is not suitable for subclassing.

## Topics

### Creating and Initializing a New Pointer Array

init(options: NSPointerFunctions.Options)

Initializes the receiver to use the given options.

init(pointerFunctions: NSPointerFunctions)

Initializes the receiver to use the given functions.

class func strongObjects() -> NSPointerArray

Returns a new pointer array that maintains strong references to its elements.

class func weakObjects() -> NSPointerArray

Returns a new pointer array that maintains weak references to its elements.

### Managing the Collection

var count: Int

The number of elements in the receiver.

var allObjects: [Any]

All the objects in the receiver.

func pointer(at: Int) -> UnsafeMutableRawPointer?

Returns the pointer at a given index.

func addPointer(UnsafeMutableRawPointer?)

Adds a given pointer to the receiver.

func removePointer(at: Int)

Removes the pointer at a given index.

func insertPointer(UnsafeMutableRawPointer?, at: Int)

Inserts a pointer at a given index.

func replacePointer(at: Int, withPointer: UnsafeMutableRawPointer?)

Replaces the pointer at a given index.

func compact()

Removes `NULL` values from the receiver.

### Getting the Pointer Functions

var pointerFunctions: NSPointerFunctions

The functions in use by the receiver.

class NSPointerFunctions

An instance of `NSPointerFunctions` defines callout functions appropriate for managing a pointer reference held somewhere else.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSFastEnumeration
- NSObjectProtocol
- NSSecureCoding

## See Also

### Pointer Collections

class NSMapTable

A collection similar to a dictionary, but with a broader range of available memory semantics.

class NSHashTable

A collection similar to a set, but with broader range of available memory semantics.

