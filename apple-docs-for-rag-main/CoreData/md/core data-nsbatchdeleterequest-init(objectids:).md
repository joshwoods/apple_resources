

- Core Data
- NSBatchDeleteRequest
-  init(objectIDs:) 

Initializer

# init(objectIDs:)

Creates a request that deletes the managed objects with the specified identifiers.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(objectIDs objects: [NSManagedObjectID])
```

## Parameters 

`objects`  

The array that contains the identifiers of the managed objects to delete.

## Discussion

Important

The identifiers your provide must be from managed objects of the same entity type; mixing entity types results in an error when you execute the request.

## See Also

### Creating a Request

init(fetchRequest: NSFetchRequest&lt;any NSFetchRequestResult>)

Creates a request that deletes the results of the specified fetch request.

