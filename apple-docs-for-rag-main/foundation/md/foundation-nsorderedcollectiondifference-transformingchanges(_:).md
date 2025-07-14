

- Foundation
- NSOrderedCollectionDifference
-  transformingChanges(\_:) 

Instance Method

# transformingChanges(\_:)

Create a new ordered collection difference by mapping over this difference’s members, processing the change objects with the block provided.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func transformingChanges(_ block: (NSOrderedCollectionChange) -> NSOrderedCollectionChange) -> CollectionDifference
```

## Parameters 

`block`  

A block receives an ordered collection change and returns an updated change.

## Return Value

A new ordered collection difference.

