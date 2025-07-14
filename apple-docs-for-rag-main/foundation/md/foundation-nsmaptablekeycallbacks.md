

- Foundation
-  NSMapTableKeyCallBacks 

Structure

# NSMapTableKeyCallBacks

The function pointers used to configure behavior of `NSMapTable` with respect to key elements within a map table.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct NSMapTableKeyCallBacks
```

## Overview

All functions must know the types of things in the map table to be able to operate on them. Sets of predefined call backs are described in NSMapTable.

Two predefined values to use for `notAKeyMarker` are NSNotAnIntMapKey and NSNotAPointerMapKey.

## Topics

### Initializers

init()

init(hash: ((NSMapTable&lt;AnyObject, AnyObject>, UnsafeRawPointer) -> Int)?, isEqual: ((NSMapTable&lt;AnyObject, AnyObject>, UnsafeRawPointer, UnsafeRawPointer) -> ObjCBool)?, retain: ((NSMapTable&lt;AnyObject, AnyObject>, UnsafeRawPointer) -> Void)?, release: ((NSMapTable&lt;AnyObject, AnyObject>, UnsafeMutableRawPointer) -> Void)?, describe: ((NSMapTable&lt;AnyObject, AnyObject>, UnsafeRawPointer) -> String?)?, notAKeyMarker: UnsafeRawPointer?)

### Instance Properties

var describe: ((NSMapTable&lt;AnyObject, AnyObject>, UnsafeRawPointer) -> String?)?

Points to the function which produces an autoreleased NSString \* describing the given element. If `NULL`, then the map table produces a generic string description.

var hash: ((NSMapTable&lt;AnyObject, AnyObject>, UnsafeRawPointer) -> Int)?

Points to the function which must produce hash code for key elements of the map table. If `NULL`, the pointer value is used as the hash code. Second parameter is the element for which hash code should be produced.

var isEqual: ((NSMapTable&lt;AnyObject, AnyObject>, UnsafeRawPointer, UnsafeRawPointer) -> ObjCBool)?

Points to the function which compares second and third parameters. If `NULL`, then == is used for comparison.

var notAKeyMarker: UnsafeRawPointer?

No key put in map table can be this value. An exception is raised if attempt is made to use this value as a key

var release: ((NSMapTable&lt;AnyObject, AnyObject>, UnsafeMutableRawPointer) -> Void)?

Points to the function which decrements a reference count for the given element, and if the reference count becomes zero, frees the given element. If `NULL`, then nothing is done for reference counting or releasing.

var retain: ((NSMapTable&lt;AnyObject, AnyObject>, UnsafeRawPointer) -> Void)?

Points to the function which increments a reference count for the given element. If `NULL`, then nothing is done for reference counting.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Data Types

struct NSMapEnumerator

Allows successive elements of a map table to be returned each time this structure is passed to NSNextMapEnumeratorPair(_:_:_:).

NSMapTable

The opaque data type used by the functions described in Managing Map Tables.

typealias NSMapTableOptions

Constants used as components in a bitfield to specify the behavior of elements (keys and values) in an `NSMapTable` object.

struct NSMapTableValueCallBacks

The function pointers used to configure behavior of `NSMapTable` with respect to value elements within a map table.

