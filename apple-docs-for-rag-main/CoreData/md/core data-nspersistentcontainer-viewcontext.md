

- Core Data
- NSPersistentContainer
-  viewContext 

Instance Property

# viewContext

The main queue’s managed object context.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var viewContext: NSManagedObjectContext { get }
```

## Mentioned in 

Setting up a Core Data stack

Syncing a Core Data Store with CloudKit

Using Core Data in the background

## Discussion

This property contains a reference to the NSManagedObjectContext that is created and owned by the persistent container which is associated with the main queue of the application. This context is created automatically as part of the initialization of the persistent container.

This context is associated directly with the NSPersistentStoreCoordinator and is non-generational by default.

## See Also

### Acquiring Contexts

func newBackgroundContext() -> NSManagedObjectContext

Returns a new managed object context that executes on a private queue.

