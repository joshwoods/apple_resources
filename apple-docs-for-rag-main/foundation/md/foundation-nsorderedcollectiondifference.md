

- Foundation
-  NSOrderedCollectionDifference 

Class

# NSOrderedCollectionDifference

An object representing the difference between two ordered collections.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class NSOrderedCollectionDifference
```

## Overview

Use differenceFromArray: or one of its variations to get an instance of NSOrderedCollectionDifference, which represents the difference between two ordered collections.

For example, the following sample compares two arrays of strings to create a difference that represents the changes:

```
NSArray *original = @[@"Red", @"Green", @"Blue"];
NSArray *modified = @[@"Red", @"Blue", @"Green"];

NSOrderedCollectionDifference *diff = [original differenceFromArray:modified];

// diff.hasChanges == TRUE
// diff.insertions.count == 1
// diff.removals.count == 1

```

## Topics

### Accessing Changes

var hasChanges: Bool

A Boolean value that indicates if the difference has changes.

var insertions: [NSOrderedCollectionChange]

A collection of insertion change objects.

var removals: [NSOrderedCollectionChange]

A collection of removal change objects.

class NSOrderedCollectionChange

An object that represents an indexed change within an ordered collection.

enum NSCollectionChangeType

The type of change represented in computing the difference of an ordered collection.

### Inverting a Difference Object

func inverse() -> Self

Calculate the difference between two objects in the reverse direction of comparison.

### Creating a Collection Difference Object

convenience init(changes: [NSOrderedCollectionChange])

Creates an ordered collection difference using an array of ordered collection changes.

convenience init(insert: IndexSet, insertedObjects: [Any]?, remove: IndexSet, removedObjects: [Any]?)

Creates an ordered collection difference from arrays of inserted and removed objects with corresponding sets of indices.

init(insert: IndexSet, insertedObjects: [Any]?, remove: IndexSet, removedObjects: [Any]?, additionalChanges: [NSOrderedCollectionChange])

Creates an ordered collection difference from arrays of inserted and removed objects with corresponding sets of indices, in addition to an array of ordered collection changes.

### Updating Changes from a Difference Object

func transformingChanges((NSOrderedCollectionChange) -> NSOrderedCollectionChange) -> CollectionDifference&lt;Any>

Create a new ordered collection difference by mapping over this difference’s members, processing the change objects with the block provided.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSFastEnumeration
- NSObjectProtocol

## See Also

### Comparing with Another Array

struct NSOrderedCollectionDifferenceCalculationOptions

Constants that specify the options to use when creating an ordered collection difference.

