

- Foundation
-  NSMapTableValueCallBacks 

Structure

# NSMapTableValueCallBacks

The function pointers used to configure behavior of `NSMapTable` with respect to value elements within a map table.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct NSMapTableValueCallBacks
```

## Overview

All functions must know the types of things in the map table to be able to operate on them. Sets of predefined call backs are described in NSMapTable.

## Topics

### Initializers

init()

init(retain: ((NSMapTable&lt;AnyObject, AnyObject>, UnsafeRawPointer) -> Void)?, release: ((NSMapTable&lt;AnyObject, AnyObject>, UnsafeMutableRawPointer) -> Void)?, describe: ((NSMapTable&lt;AnyObject, AnyObject>, UnsafeRawPointer) -> String?)?)

### Instance Properties

var describe: ((NSMapTable&lt;AnyObject, AnyObject>, UnsafeRawPointer) -> String?)?

Points to the function that produces an autoreleased NSString \* describing the given element. If `NULL`, then the map table produces a generic string description.

var release: ((NSMapTable&lt;AnyObject, AnyObject>, UnsafeMutableRawPointer) -> Void)?

Points to the function that decrements a reference count for the given element, and if the reference count becomes zero, frees the given element. If `NULL`, then nothing is done for reference counting or releasing.

var retain: ((NSMapTable&lt;AnyObject, AnyObject>, UnsafeRawPointer) -> Void)?

Points to the function that increments a reference count for the given element. If `NULL`, then nothing is done for reference counting.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Data Types

struct NSMapEnumerator

Allows successive elements of a map table to be returned each time this structure is passed to NSNextMapEnumeratorPair(_:_:_:).

NSMapTable

The opaque data type used by the functions described in Managing Map Tables.

struct NSMapTableKeyCallBacks

The function pointers used to configure behavior of `NSMapTable` with respect to key elements within a map table.

typealias NSMapTableOptions

Constants used as components in a bitfield to specify the behavior of elements (keys and values) in an `NSMapTable` object.

