

- AppKit
- NSController
-  commitEditing() 

Instance Method

# commitEditing()

Causes the receiver to attempt to commit any pending edits, returning true if successful or no edits were pending.

macOS

``` source
@MainActor
func commitEditing() -> Bool
```

## Discussion

The receiver invokes commitEditing on any current editors, returning their response. A commit is denied if the receiver fails to apply the changes to the model object, perhaps due to a validation error.

## See Also

### Managing editing

func objectDidBeginEditing(any NSEditor)

Invoked to inform the receiver that `editor` has uncommitted changes that can affect the receiver.

func objectDidEndEditing(any NSEditor)

Invoked to inform the receiver that `editor` has committed or discarded its changes.

func commitEditing(withDelegate: Any?, didCommit: Selector?, contextInfo: UnsafeMutableRawPointer?)

Attempts to commit any pending changes in known editors of the receiver.

func discardEditing()

Discards any pending changes by registered editors.

var isEditing: Bool

A Boolean value indicating if any editors are registered with the controller.

