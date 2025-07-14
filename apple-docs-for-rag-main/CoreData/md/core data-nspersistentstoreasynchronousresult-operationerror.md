

- Core Data
- NSPersistentStoreAsynchronousResult
-  operationError 

Instance Property

# operationError

An error that contains details if the asynchronous fetch request fails.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var operationError: (any Error)? { get }
```

## See Also

### Inspecting the Result

var managedObjectContext: NSManagedObjectContext

The managed object context for the result.

var progress: Progress?

An object that reports progress for the asynchronous fetch request.

