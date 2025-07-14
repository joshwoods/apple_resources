

- AppKit
- NSViewController
-  commitEditing() 

Instance Method

# commitEditing()

Returns whether the receiver was able to commit any pending edits.

macOS 10.5+

``` source
@MainActor
func commitEditing() -> Bool
```

## Return Value

Returns true if the changes were successfully applied to the model, false otherwise.

## Discussion

A commit is denied if the receiver fails to apply the changes to the model object, perhaps due to a validation error.

## See Also

### NSEditor Conformance

func commitEditing(withDelegate: Any?, didCommit: Selector?, contextInfo: UnsafeMutableRawPointer?)

Attempt to commit any currently edited results of the receiver.

func discardEditing()

Causes the receiver to discard any changes, restoring the previous values.

