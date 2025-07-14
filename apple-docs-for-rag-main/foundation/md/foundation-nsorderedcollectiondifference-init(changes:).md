

- Foundation
- NSOrderedCollectionDifference
-  init(changes:) 

Initializer

# init(changes:)

Creates an ordered collection difference using an array of ordered collection changes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
convenience init(changes: [NSOrderedCollectionChange])
```

## Parameters 

`changes`  

An array of ordered collection changes.

## See Also

### Creating a Collection Difference Object

convenience init(insert: IndexSet, insertedObjects: [Any]?, remove: IndexSet, removedObjects: [Any]?)

Creates an ordered collection difference from arrays of inserted and removed objects with corresponding sets of indices.

init(insert: IndexSet, insertedObjects: [Any]?, remove: IndexSet, removedObjects: [Any]?, additionalChanges: [NSOrderedCollectionChange])

Creates an ordered collection difference from arrays of inserted and removed objects with corresponding sets of indices, in addition to an array of ordered collection changes.

