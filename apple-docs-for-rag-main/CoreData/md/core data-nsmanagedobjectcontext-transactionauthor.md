

- Core Data
- NSManagedObjectContext
-  transactionAuthor 

Instance Property

# transactionAuthor

The author for the context that is used as an identifier in persistent history transactions.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var transactionAuthor: String? { get set }
```

## Mentioned in 

Consuming relevant store changes

## Discussion

Set a managed object context’s transactionAuthor before saving it to differentiate among multiple call sites that modify the same context. Doing this records an author in subsequent transactions.

```
func addColor(_ name: String, in context: NSManagedObjectContext) {
    let color = Color(context: context)
    color.name = name
    color.creationDate = Date()

    // set the transaction author
    context.transactionAuthor = "addColor"
    persistentContainer.saveContext(context)
    context.transactionAuthor = nil
}
```

Reset the context’s transactionAuthor to nil after the save to prevent misattribution of future transactions.

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

func mergeChanges(fromContextDidSave: Notification)

Merges the changes specified in a given notification.

func setQueryGenerationFrom(NSQueryGenerationToken?) throws

Sets the query generation this context should use.

