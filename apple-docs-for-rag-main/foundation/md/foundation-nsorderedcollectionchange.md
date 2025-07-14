

- Foundation
-  NSOrderedCollectionChange 

Class

# NSOrderedCollectionChange

An object that represents an indexed change within an ordered collection.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class NSOrderedCollectionChange
```

## Overview

An ordered collection change represents changes by adding, removing, or moving objects within an ordered collection. Changes with an associated index indicate a move within the collection.

## Topics

### Creating a Change

convenience init(object: Any?, type: NSCollectionChangeType, index: Int)

Creates a change object that represents inserting or removing an object from an ordered collection at a specific index.

init(object: Any?, type: NSCollectionChangeType, index: Int, associatedIndex: Int)

Creates a change object that represents inserting, removing, or moving an object from an ordered collection at a specific index.

### Accessing the Change

var changeType: NSCollectionChangeType

The type of change.

var index: Int

The index location of the change.

var object: Any?

An object the change inserts or removes.

var associatedIndex: Int

When this property is set to a value other than NSNotFound, the receiver is one half of a move, and this value is the index of the change’s counterpart of the opposite type in the diff.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Accessing Changes

var hasChanges: Bool

A Boolean value that indicates if the difference has changes.

var insertions: [NSOrderedCollectionChange]

A collection of insertion change objects.

var removals: [NSOrderedCollectionChange]

A collection of removal change objects.

enum NSCollectionChangeType

The type of change represented in computing the difference of an ordered collection.

