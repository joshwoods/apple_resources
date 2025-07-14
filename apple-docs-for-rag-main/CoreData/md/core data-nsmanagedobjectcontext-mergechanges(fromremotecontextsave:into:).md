

- Core Data
- NSManagedObjectContext
-  mergeChanges(fromRemoteContextSave:into:) 

Type Method

# mergeChanges(fromRemoteContextSave:into:)

Handles changes from other processes or from a serialized state.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func mergeChanges(
    fromRemoteContextSave changeNotificationData: [AnyHashable : Any],
    into contexts: [NSManagedObjectContext]
)
```

## Mentioned in 

Accessing data when the store changes

## Discussion

This method more efficiently merges changes into multiple contexts as well as nested contexts. The dictionary keys should be one or more from an NSManagedObjectContextObjectsDidChange: NSInsertedObjectsKey, NSUpdatedObjectsKey, NSDeletedObjectsKey. The values should be an NSArray of either NSManagedObjectID or NSURL objects conforming to valid results from uriRepresentation().

## See Also

### Managing concurrency

let NSManagedObjectContextQueryGenerationKey: String

Constant used to reference the query generation token.

var automaticallyMergesChangesFromParent: Bool

A Boolean value that indicates whether the context automatically merges changes saved to its persistent store coordinator or parent context.

var concurrencyType: NSManagedObjectContextConcurrencyType

The concurrency type for the context.

var mergePolicy: Any

The merge policy of the context.

var queryGenerationToken: NSQueryGenerationToken?

Returns the token associated with the query generation currently in use by this context.

var transactionAuthor: String?

The author for the context that is used as an identifier in persistent history transactions.

func mergeChanges(fromContextDidSave: Notification)

Merges the changes specified in a given notification.

func setQueryGenerationFrom(NSQueryGenerationToken?) throws

Sets the query generation this context should use.

