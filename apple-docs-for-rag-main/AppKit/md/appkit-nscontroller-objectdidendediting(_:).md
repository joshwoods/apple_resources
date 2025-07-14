

- AppKit
- NSController
-  objectDidEndEditing(\_:) 

Instance Method

# objectDidEndEditing(\_:)

Invoked to inform the receiver that `editor` has committed or discarded its changes.

macOS

``` source
@MainActor
func objectDidEndEditing(_ editor: any NSEditor)
```

## See Also

### Managing editing

func objectDidBeginEditing(any NSEditor)

Invoked to inform the receiver that `editor` has uncommitted changes that can affect the receiver.

func commitEditing() -> Bool

Causes the receiver to attempt to commit any pending edits, returning true if successful or no edits were pending.

func commitEditing(withDelegate: Any?, didCommit: Selector?, contextInfo: UnsafeMutableRawPointer?)

Attempts to commit any pending changes in known editors of the receiver.

func discardEditing()

Discards any pending changes by registered editors.

var isEditing: Bool

A Boolean value indicating if any editors are registered with the controller.

