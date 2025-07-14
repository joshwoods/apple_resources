

- Core Data
- NSManagedObjectContext
-  rollback() 

Instance Method

# rollback()

Removes everything from the undo stack, discards all insertions and deletions, and restores updated objects to their last committed values.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func rollback()
```

## Discussion

This method does not refetch data from the persistent store or stores.

## See Also

### Related Documentation

func processPendingChanges()

Forces the context to process changes to the object graph.

var stalenessInterval: TimeInterval

The maximum length of time that may have elapsed since the store previously fetched data before fulfilling a fault issues a new fetch.

### Undoing changes

var undoManager: UndoManager?

The object that provides undo support for the context.

func undo()

Sends an undo message to the context’s undo manager, asking it to reverse the latest uncommitted changes applied to objects in the object graph.

func redo()

Sends a redo message to the context’s undo manager, asking it to reverse the latest undo operation applied to objects in the object graph.

func reset()

Returns the context to its base state.

