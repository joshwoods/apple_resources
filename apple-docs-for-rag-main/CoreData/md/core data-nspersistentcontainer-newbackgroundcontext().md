

- Core Data
- NSPersistentContainer
-  newBackgroundContext() 

Instance Method

# newBackgroundContext()

Returns a new managed object context that executes on a private queue.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func newBackgroundContext() -> NSManagedObjectContext
```

## Return Value

A newly created private managed object context.

## Mentioned in 

Using Core Data in the background

## Discussion

Invoking this method causes the persistent container to create and return a new NSManagedObjectContext with the concurrencyType set to NSManagedObjectContextConcurrencyType.privateQueueConcurrencyType. This new context will be associated with the NSPersistentStoreCoordinator directly and is set to consume NSManagedObjectContextDidSave broadcasts automatically.

## See Also

### Acquiring Contexts

var viewContext: NSManagedObjectContext

The main queue’s managed object context.

