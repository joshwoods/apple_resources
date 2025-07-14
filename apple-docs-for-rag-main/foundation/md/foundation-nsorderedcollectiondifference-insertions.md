

- Foundation
- NSOrderedCollectionDifference
-  insertions 

Instance Property

# insertions

A collection of insertion change objects.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var insertions: [NSOrderedCollectionChange] { get }
```

## See Also

### Accessing Changes

var hasChanges: Bool

A Boolean value that indicates if the difference has changes.

var removals: [NSOrderedCollectionChange]

A collection of removal change objects.

class NSOrderedCollectionChange

An object that represents an indexed change within an ordered collection.

enum NSCollectionChangeType

The type of change represented in computing the difference of an ordered collection.

