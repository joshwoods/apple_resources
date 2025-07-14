

- Foundation
-  NSHashTableCallBacks 

Structure

# NSHashTableCallBacks

Defines a structure that contains the function pointers used to configure behavior of `NSHashTable` with respect to elements within a hash table.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct NSHashTableCallBacks
```

## Overview

All functions must know the types of things in the hash table to be able to operate on them. Sets of predefined call backs are described in NSHashTable.

## Topics

### Initializers

init()

init(hash: ((NSHashTable&lt;AnyObject>, UnsafeRawPointer) -> Int)?, isEqual: ((NSHashTable&lt;AnyObject>, UnsafeRawPointer, UnsafeRawPointer) -> ObjCBool)?, retain: ((NSHashTable&lt;AnyObject>, UnsafeRawPointer) -> Void)?, release: ((NSHashTable&lt;AnyObject>, UnsafeMutableRawPointer) -> Void)?, describe: ((NSHashTable&lt;AnyObject>, UnsafeRawPointer) -> String?)?)

### Instance Properties

var describe: ((NSHashTable&lt;AnyObject>, UnsafeRawPointer) -> String?)?

Points to the function that produces an autoreleased NSString \* describing the given element. If `NULL`, then the hash table produces a generic string description.

var hash: ((NSHashTable&lt;AnyObject>, UnsafeRawPointer) -> Int)?

Points to the function that must produce hash code for elements of the hash table. If `NULL`, the pointer value is used as the hash code. Second parameter is the element for which hash code should be produced.

var isEqual: ((NSHashTable&lt;AnyObject>, UnsafeRawPointer, UnsafeRawPointer) -> ObjCBool)?

Points to the function that compares second and third parameters. If `NULL`, then == is used for comparison.

var release: ((NSHashTable&lt;AnyObject>, UnsafeMutableRawPointer) -> Void)?

Points to the function that decrements a reference count for the given element, and if the reference count becomes 0, frees the given element. If `NULL`, then nothing is done for reference counting or releasing.

var retain: ((NSHashTable&lt;AnyObject>, UnsafeRawPointer) -> Void)?

Points to the function that increments a reference count for the given element. If `NULL`, then nothing is done for reference counting.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Data Types

struct NSHashEnumerator

Allows successive elements of a hash table to be returned each time this structure is passed to NSNextHashEnumeratorItem(_:).

typealias NSHashTableOptions

Components in a bit-field to specify the behavior of elements in an NSHashTable object.

