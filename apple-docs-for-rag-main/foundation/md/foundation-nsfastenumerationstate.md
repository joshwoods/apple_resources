

- Foundation
-  NSFastEnumerationState 

Structure

# NSFastEnumerationState

This defines the structure used as contextual information in the NSFastEnumeration protocol.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct NSFastEnumerationState
```

## Overview

For more information, see countByEnumerating(with:objects:count:).

## Topics

### Initializers

init()

init(state: UInt, itemsPtr: AutoreleasingUnsafeMutablePointer&lt;AnyObject?>?, mutationsPtr: UnsafeMutablePointer&lt;UInt>?, extra: (UInt, UInt, UInt, UInt, UInt))

### Instance Properties

var extra: (UInt, UInt, UInt, UInt, UInt)

A C array that you can use to hold returned values.

var itemsPtr: AutoreleasingUnsafeMutablePointer&lt;AnyObject?>?

A C array of objects.

var mutationsPtr: UnsafeMutablePointer&lt;UInt>?

Arbitrary state information used to detect whether the collection has been mutated.

var state: UInt

Arbitrary state information used by the iterator. Typically this is set to `0` at the beginning of the iteration.

## Relationships

### Conforms To

- BitwiseCopyable

