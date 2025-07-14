

- Core Data
- NSManagedObjectContext
-  persistentStoreCoordinator 

Instance Property

# persistentStoreCoordinator

The persistent store coordinator of the context.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var persistentStoreCoordinator: NSPersistentStoreCoordinator? { get set }
```

## Return Value

The persistent store coordinator of the receiver.

## Discussion

The coordinator provides the managed object model and handles persistency. Note that multiple contexts can share a coordinator. May not be `nil`.

Setting persistentStoreCoordinator to `nil` will raise an exception. If you want to “disconnect” a context from its persistent store coordinator, you should simply set all strong references to the context to `nil` and allow it to be deallocated normally.

For more details, see Parent store.

## See Also

### Configuring a context

var parent: NSManagedObjectContext?

The parent of the context.

var name: String?

The developer-provided name of the context.

var userInfo: NSMutableDictionary

The user information for the context.

