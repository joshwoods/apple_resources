

- Core Data
- NSPersistentStore
-  willRemove(from:) 

Instance Method

# willRemove(from:)

Invoked before the persistent store is removed from the persistent store coordinator.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func willRemove(from coordinator: NSPersistentStoreCoordinator?)
```

## Parameters 

`coordinator`  

The persistent store coordinator from which the receiver was removed.

## Discussion

The default implementation does nothing. You can override this method in a subclass in order to perform any clean-up before the store is removed from the coordinator (and deallocated).

## See Also

### Responding to the Store Life Cycle

func didAdd(to: NSPersistentStoreCoordinator)

Invoked after the persistent store has been added to the persistent store coordinator.

