

- SwiftData
- ModelContext
-  save() 

Instance Method

# save()

Writes any pending inserts, changes, and deletes to the persistent storage.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
func save() throws
```

## Mentioned in 

Preserving your app’s model data across launches

## Discussion

Important

Use the hasChanges property to determine whether the context has uncommitted changes before invoking this method. Otherwise, SwiftData may perform unnecessary work.

## See Also

### Persisting unsaved changes

var autosaveEnabled: Bool

A Boolean value that indicates whether the context should automatically save any pending changes when certain events occur.

func transaction(block: () throws -> Void) throws

Runs the provided closure, and once it finishes, writes any pending inserts, changes, and deletes to the persistent storage.

func rollback()

Discards pending inserts and deletes, restores changed models to their most recent committed state, and empties the undo stack.

