

- AppKit
- NSViewController
-  discardEditing() 

Instance Method

# discardEditing()

Causes the receiver to discard any changes, restoring the previous values.

macOS 10.5+

``` source
@MainActor
func discardEditing()
```

## See Also

### NSEditor Conformance

func commitEditing(withDelegate: Any?, didCommit: Selector?, contextInfo: UnsafeMutableRawPointer?)

Attempt to commit any currently edited results of the receiver.

func commitEditing() -> Bool

Returns whether the receiver was able to commit any pending edits.

