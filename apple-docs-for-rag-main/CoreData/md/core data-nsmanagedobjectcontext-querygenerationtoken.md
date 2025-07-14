

- Core Data
- NSManagedObjectContext
-  queryGenerationToken 

Instance Property

# queryGenerationToken

Returns the token associated with the query generation currently in use by this context.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var queryGenerationToken: NSQueryGenerationToken? { get }
```

## Mentioned in 

Accessing data when the store changes

## See Also

### Managing concurrency

let NSManagedObjectContextQueryGenerationKey: String

Constant used to reference the query generation token.

class func mergeChanges(fromRemoteContextSave: [AnyHashable : Any], into: [NSManagedObjectContext])

Handles changes from other processes or from a serialized state.

var automaticallyMergesChangesFromParent: Bool

A Boolean value that indicates whether the context automatically merges changes saved to its persistent store coordinator or parent context.

var concurrencyType: NSManagedObjectContextConcurrencyType

The concurrency type for the context.

var mergePolicy: Any

The merge policy of the context.

var transactionAuthor: String?

The author for the context that is used as an identifier in persistent history transactions.

func mergeChanges(fromContextDidSave: Notification)

Merges the changes specified in a given notification.

func setQueryGenerationFrom(NSQueryGenerationToken?) throws

Sets the query generation this context should use.

