

- Core Data
- NSPersistentStoreAsynchronousResult
-  managedObjectContext 

Instance Property

# managedObjectContext

The managed object context for the result.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var managedObjectContext: NSManagedObjectContext { get }
```

## See Also

### Inspecting the Result

var operationError: (any Error)?

An error that contains details if the asynchronous fetch request fails.

var progress: Progress?

An object that reports progress for the asynchronous fetch request.

