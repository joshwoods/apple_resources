

- Core Data
- NSManagedObjectContext
-  mergeChanges(fromContextDidSave:) 

Instance Method

# mergeChanges(fromContextDidSave:)

Merges the changes specified in a given notification.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func mergeChanges(fromContextDidSave notification: Notification)
```

## Parameters 

`notification`  

An instance of an NSManagedObjectContextDidSave notification posted by another context.

## Mentioned in 

Consuming relevant store changes

Accessing data when the store changes

## Discussion

This method refreshes any objects which have been updated in the other context, faults in any newly-inserted objects, and invokes delete(_:): on those which have been deleted.

You can pass a NSManagedObjectContextDidSave notification posted by a managed object context on another thread, however you must not use the managed objects in the user info dictionary directly. For more details, see Concurrency with Core Data.

Note

Objective-C uses instances of NSManagedObjectContextDidSaveNotification instead of NSManagedObjectContextDidSave.

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

var queryGenerationToken: NSQueryGenerationToken?

Returns the token associated with the query generation currently in use by this context.

var transactionAuthor: String?

The author for the context that is used as an identifier in persistent history transactions.

func setQueryGenerationFrom(NSQueryGenerationToken?) throws

Sets the query generation this context should use.

