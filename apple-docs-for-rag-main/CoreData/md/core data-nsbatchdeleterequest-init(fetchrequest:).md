

- Core Data
- NSBatchDeleteRequest
-  init(fetchRequest:) 

Initializer

# init(fetchRequest:)

Creates a request that deletes the results of the specified fetch request.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(fetchRequest fetch: NSFetchRequest)
```

## Parameters 

`fetch`  

The fetch request that identifies the managed objects to delete.

## See Also

### Creating a Request

convenience init(objectIDs: [NSManagedObjectID])

Creates a request that deletes the managed objects with the specified identifiers.

