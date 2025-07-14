

- Core Data
- NSPersistentStore
-  didAdd(to:) 

Instance Method

# didAdd(to:)

Invoked after the persistent store has been added to the persistent store coordinator.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func didAdd(to coordinator: NSPersistentStoreCoordinator)
```

## Parameters 

`coordinator`  

The persistent store coordinator to which the receiver was added.

## Discussion

The default implementation does nothing. You can override this method in a subclass in order to perform any kind of setup necessary before the load method is invoked.

## See Also

### Responding to the Store Life Cycle

func willRemove(from: NSPersistentStoreCoordinator?)

Invoked before the persistent store is removed from the persistent store coordinator.

