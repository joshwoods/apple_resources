

- Core Data
- NSManagedObjectContext
-  parent 

Instance Property

# parent

The parent of the context.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var parent: NSManagedObjectContext? { get set }
```

## Discussion

`nil` indicates there is no parent context. For more details, see Parent store.

## See Also

### Configuring a context

var persistentStoreCoordinator: NSPersistentStoreCoordinator?

The persistent store coordinator of the context.

var name: String?

The developer-provided name of the context.

var userInfo: NSMutableDictionary

The user information for the context.

