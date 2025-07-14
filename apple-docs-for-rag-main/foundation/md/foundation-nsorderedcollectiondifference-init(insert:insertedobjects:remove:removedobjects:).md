

- Foundation
- NSOrderedCollectionDifference
-  init(insert:insertedObjects:remove:removedObjects:) 

Initializer

# init(insert:insertedObjects:remove:removedObjects:)

Creates an ordered collection difference from arrays of inserted and removed objects with corresponding sets of indices.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
convenience init(
    insert inserts: IndexSet,
    insertedObjects: [Any]?,
    remove removes: IndexSet,
    removedObjects: [Any]?
)
```

## Parameters 

`inserts`  

An index set that represents the index values to associate with the objects in the provided array of inserted objects.

`insertedObjects`  

An array of objects the ordered collection difference will insert.

`removes`  

An index set that represents the index values to associate with the objects in the provided array of removed objects.

`removedObjects`  

An array of objects the ordered collection difference will remove.

## See Also

### Creating a Collection Difference Object

convenience init(changes: [NSOrderedCollectionChange])

Creates an ordered collection difference using an array of ordered collection changes.

init(insert: IndexSet, insertedObjects: [Any]?, remove: IndexSet, removedObjects: [Any]?, additionalChanges: [NSOrderedCollectionChange])

Creates an ordered collection difference from arrays of inserted and removed objects with corresponding sets of indices, in addition to an array of ordered collection changes.

