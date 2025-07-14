

- Core Data
- NSBatchDeleteRequest
-  fetchRequest 

Instance Property

# fetchRequest

The fetch request that identifies the managed objects to delete.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@NSCopying
var fetchRequest: NSFetchRequest { get }
```

## Discussion

This property contains the fetch request that identifies the managed objects to delete. If you initialize `NSBatchDeleteRequest` with an array of NSManagedObjectID, Core Data automatically generates a fetch request with a predicate that matches the identifiers in that array.

