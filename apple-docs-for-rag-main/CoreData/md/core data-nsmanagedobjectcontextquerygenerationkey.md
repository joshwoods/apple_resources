

- Core Data
-  NSManagedObjectContextQueryGenerationKey 

Global Variable

# NSManagedObjectContextQueryGenerationKey

Constant used to reference the query generation token.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
let NSManagedObjectContextQueryGenerationKey: String
```

## See Also

### Managing concurrency

class func mergeChanges(fromRemoteContextSave: [AnyHashable : Any], into: [NSManagedObjectContext])

Handles changes from other processes or from a serialized state.

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

