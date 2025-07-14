

- Foundation
-  NSPointerFunctions 

Class

# NSPointerFunctions

An instance of `NSPointerFunctions` defines callout functions appropriate for managing a pointer reference held somewhere else.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSPointerFunctions
```

## Overview

The functions specified by an instance of `NSPointerFunctions` are separated into two clusters—those that define “personality” such as “object” or “C-string”, and those that describe memory management issues such as a memory deallocation function. There are constants for common personalities and memory manager selections (see `Memory and Personality Options`).

NSHashTable, NSMapTable, and NSPointerArray use an `NSPointerFunctions` object to define the acquisition and retention behavior for the pointers they manage. Note, however, that not all combinations of personality and memory management behavior are valid for these collections. The pointer collection objects copy the `NSPointerFunctions` object on input and output, so you cannot usefully subclass `NSPointerFunctions`.

### Subclassing Notes

`NSPointerFunctions` is not suitable for subclassing.

## Topics

### Creating and Initializing an NSPointerFunctions Object

init(options: NSPointerFunctions.Options)

Returns an `NSPointerFunctions` object initialized with the given options.

### Personality Functions

var hashFunction: ((UnsafeRawPointer, ((UnsafeRawPointer) -> Int)?) -> Int)?

The hash function.

var isEqualFunction: ((UnsafeRawPointer, UnsafeRawPointer, ((UnsafeRawPointer) -> Int)?) -> ObjCBool)?

The function used to compare pointers.

var sizeFunction: ((UnsafeRawPointer) -> Int)?

The function used to determine the size of pointers.

var descriptionFunction: ((UnsafeRawPointer) -> String?)?

### Memory Configuration

var acquireFunction: ((UnsafeRawPointer, ((UnsafeRawPointer) -> Int)?, ObjCBool) -> UnsafeMutableRawPointer)?

The function used to acquire memory.

var relinquishFunction: ((UnsafeRawPointer, ((UnsafeRawPointer) -> Int)?) -> Void)?

The function used to relinquish memory.

var usesStrongWriteBarrier: Bool

Specifies whether, in a garbage collected environment, pointers should be assigned using a strong write barrier.

Deprecated

var usesWeakReadAndWriteBarriers: Bool

Specifies whether, in a garbage collected environment, pointers should use weak read and write barriers.

Deprecated

### Constants

struct Options

Defines the memory and personality options for an `NSPointerFunctions` object.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Accessing Pointer Functions

var pointerFunctions: NSPointerFunctions

The pointer functions for the hash table.

