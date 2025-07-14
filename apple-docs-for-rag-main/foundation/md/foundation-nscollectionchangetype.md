

- Foundation
-  NSCollectionChangeType 

Enumeration

# NSCollectionChangeType

The type of change represented in computing the difference of an ordered collection.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum NSCollectionChangeType
```

## Topics

### Types of Ordered Collection Changes

case insert

A change type that represents the insertion of an object into an ordered collection.

case remove

A change type that represents the removal of an object from an ordered collection.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessing Changes

var hasChanges: Bool

A Boolean value that indicates if the difference has changes.

var insertions: [NSOrderedCollectionChange]

A collection of insertion change objects.

var removals: [NSOrderedCollectionChange]

A collection of removal change objects.

class NSOrderedCollectionChange

An object that represents an indexed change within an ordered collection.

