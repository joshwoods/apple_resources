

- SwiftData
- ModelContext
-  rollback() 

Instance Method

# rollback()

Discards pending inserts and deletes, restores changed models to their most recent committed state, and empties the undo stack.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
func rollback()
```

## See Also

### Persisting unsaved changes

var autosaveEnabled: Bool

A Boolean value that indicates whether the context should automatically save any pending changes when certain events occur.

func save() throws

Writes any pending inserts, changes, and deletes to the persistent storage.

func transaction(block: () throws -> Void) throws

Runs the provided closure, and once it finishes, writes any pending inserts, changes, and deletes to the persistent storage.

