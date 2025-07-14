

- AppKit
- NSController
-  objectDidBeginEditing(\_:) 

Instance Method

# objectDidBeginEditing(\_:)

Invoked to inform the receiver that `editor` has uncommitted changes that can affect the receiver.

macOS

``` source
@MainActor
func objectDidBeginEditing(_ editor: any NSEditor)
```

## See Also

### Related Documentation

Cocoa Bindings Programming Topics

### Managing editing

func objectDidEndEditing(any NSEditor)

Invoked to inform the receiver that `editor` has committed or discarded its changes.

func commitEditing() -> Bool

Causes the receiver to attempt to commit any pending edits, returning true if successful or no edits were pending.

func commitEditing(withDelegate: Any?, didCommit: Selector?, contextInfo: UnsafeMutableRawPointer?)

Attempts to commit any pending changes in known editors of the receiver.

func discardEditing()

Discards any pending changes by registered editors.

var isEditing: Bool

A Boolean value indicating if any editors are registered with the controller.

