

- Core Data
- NSManagedObjectContext
-  mergePolicy 

Instance Property

# mergePolicy

The merge policy of the context.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var mergePolicy: Any { get set }
```

## Discussion

The default is NSErrorMergePolicy. For possible values, see NSMergePolicy.

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

var queryGenerationToken: NSQueryGenerationToken?

Returns the token associated with the query generation currently in use by this context.

var transactionAuthor: String?

The author for the context that is used as an identifier in persistent history transactions.

func mergeChanges(fromContextDidSave: Notification)

Merges the changes specified in a given notification.

func setQueryGenerationFrom(NSQueryGenerationToken?) throws

Sets the query generation this context should use.

