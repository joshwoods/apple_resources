

- Foundation
-  NSMutableCopying 

Protocol

# NSMutableCopying

A protocol that mutable objects adopt to provide functional copies of themselves.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol NSMutableCopying
```

## Overview

The NSMutableCopying protocol declares a method for providing mutable copies of an object. Only classes that define an “immutable vs. mutable” distinction should adopt this protocol. Classes that don’t define such a distinction should adopt NSCopying instead.

NSMutableCopying declares one method, mutableCopy(with:), but mutable copying is commonly invoked with the convenience method mutableCopy(). The mutableCopy() method is defined for all NSObjects and simply invokes mutableCopy(with:) with the default zone.

If a subclass inherits NSMutableCopying from its superclass and declares additional instance variables, the subclass has to override mutableCopy(with:) to properly handle its own instance variables, invoking the superclass’s implementation first.

## Topics

### Copying

func mutableCopy(with: NSZone?) -> Any

Returns a new instance that’s a mutable copy of the receiver.

**Required**

## Relationships

### Conforming Types

- NSArray
- NSAttributedString
- NSCharacterSet
- NSCountedSet
- NSData
- NSDictionary
- NSIndexSet
- NSMutableArray
- NSMutableAttributedString
- NSMutableCharacterSet
- NSMutableData
- NSMutableDictionary
- NSMutableIndexSet
- NSMutableOrderedSet
- NSMutableSet
- NSMutableString
- NSMutableURLRequest
- NSOrderedSet
- NSPurgeableData
- NSSet
- NSString
- NSURLRequest

## See Also

### Copying

protocol NSCopying

A protocol that objects adopt to provide functional copies of themselves.

