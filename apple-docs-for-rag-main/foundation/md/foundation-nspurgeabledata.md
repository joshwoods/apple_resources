

- Foundation
-  NSPurgeableData 

Class

# NSPurgeableData

A mutable data object containing bytes that can be discarded when they’re no longer needed.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSPurgeableData
```

## Overview

NSPurgeableData objects inherit their creation methods from their superclass, NSMutableData while providing a default implementation of the NSDiscardableContent protocol.

All NSPurgeableData objects begin “accessed” to ensure that they are not instantly discarded. The beginContentAccess() method marks the object’s bytes as “accessed,” thus protecting them from being discarded, and must be called before accessing the object, or else an exception will be raised. This method returns true if the bytes have not been discarded and if they have been successfully marked as “accessed”. Any method that directly or indirectly accesses these bytes or their length when they are not “accessed” will raise an exception. When you are done with the data, call endContentAccess() to allow them to be discarded in order to quickly free up memory.

You may use these objects by themselves, and do not necessarily have to use them in conjunction with NSCache to get the purging behavior. The NSCache class incorporates a caching mechanism with some auto-removal policies to ensure that its memory footprint does not get too large.

NSPurgeableData objects should not be used as keys in hashing-based collections, because the value of the bytes pointer can change after every mutation of the data.

## Relationships

### Inherits From

- NSMutableData

### Conforms To

- BidirectionalCollection
- CVarArg
- Collection
- CustomDebugStringConvertible
- CustomStringConvertible
- DataProtocol
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSDiscardableContent
- NSMutableCopying
- NSObjectProtocol
- NSSecureCoding
- RandomAccessCollection
- Sequence

## See Also

### Purgeable Collections

class NSCache

A mutable collection you use to temporarily store transient key-value pairs that are subject to eviction when resources are low.

