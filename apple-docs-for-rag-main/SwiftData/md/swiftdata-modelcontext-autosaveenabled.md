

- SwiftData
- ModelContext
-  autosaveEnabled 

Instance Property

# autosaveEnabled

A Boolean value that indicates whether the context should automatically save any pending changes when certain events occur.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
var autosaveEnabled: Bool { get set }
```

## Mentioned in 

Preserving your app’s model data across launches

## Discussion

When `true`, the context calls save() after you make changes to any inserted or registered models. The context also calls `save()` at various times during the lifecycle of windows, scenes, views, and sheets.

The default value is `false`. SwiftData automatically sets this property to `true` for the model container’s mainContext.

## See Also

### Persisting unsaved changes

func save() throws

Writes any pending inserts, changes, and deletes to the persistent storage.

func transaction(block: () throws -> Void) throws

Runs the provided closure, and once it finishes, writes any pending inserts, changes, and deletes to the persistent storage.

func rollback()

Discards pending inserts and deletes, restores changed models to their most recent committed state, and empties the undo stack.

