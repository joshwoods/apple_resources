

- Foundation
-  NSMutableIndexSet 

Class

# NSMutableIndexSet

A mutable collection of unique integer values that represent indexes in another collection.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSMutableIndexSet
```

## Overview

In Swift, this type bridges to IndexSet; use NSMutableIndexSet when you need reference semantics or other Foundation-specific behavior.

The NSMutableIndexSet class represents a mutable collection of unique unsigned integers, known as *indexes* because of the way they are used. This collection is referred to as a *mutable index set*. The inclusive range of valid indexes is `0...(NSNotFound - 1)`; trying to use indexes outside this range is invalid.

The values in a mutable index set are always sorted, so the order in which values are added is irrelevant.

Do not subclass the NSMutableIndexSet class.

Important

The Swift overlay to the Foundation framework provides the IndexSet structure, which bridges to the NSMutableIndexSet class and its immutable superclass, NSIndexSet. For more information about value types, see Working with Cocoa Frameworks in Using Swift with Cocoa and Objective-C (Swift 4.1).

## Topics

### Adding Indexes

func add(Int)

Adds an index to the receiver.

func add(IndexSet)

Adds the indexes in an index set to the receiver.

func add(in: NSRange)

Adds the indexes in an index range to the receiver.

### Removing Indexes

func remove(Int)

Removes an index from the receiver.

func remove(IndexSet)

Removes the indexes in an index set from the receiver.

func removeAllIndexes()

Removes the receiver’s indexes.

func remove(in: NSRange)

Removes the indexes in an index range from the receiver.

### Shifting Index Groups

func shiftIndexesStarting(at: Int, by: Int)

Shifts a group of indexes to the left or the right within the receiver.

## Relationships

### Inherits From

- NSIndexSet

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSMutableCopying
- NSObjectProtocol
- NSSecureCoding
- Sequence

