

- AppKit
- NSController
-  discardEditing() 

Instance Method

# discardEditing()

Discards any pending changes by registered editors.

macOS

``` source
@MainActor
func discardEditing()
```

## Discussion

The receiver invokes discardEditing on any current editors.

## See Also

### Managing editing

func objectDidBeginEditing(any NSEditor)

Invoked to inform the receiver that `editor` has uncommitted changes that can affect the receiver.

func objectDidEndEditing(any NSEditor)

Invoked to inform the receiver that `editor` has committed or discarded its changes.

func commitEditing() -> Bool

Causes the receiver to attempt to commit any pending edits, returning true if successful or no edits were pending.

func commitEditing(withDelegate: Any?, didCommit: Selector?, contextInfo: UnsafeMutableRawPointer?)

Attempts to commit any pending changes in known editors of the receiver.

var isEditing: Bool

A Boolean value indicating if any editors are registered with the controller.

