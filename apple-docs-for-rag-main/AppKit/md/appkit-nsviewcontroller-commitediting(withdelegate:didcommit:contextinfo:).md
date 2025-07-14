

- AppKit
- NSViewController
-  commitEditing(withDelegate:didCommit:contextInfo:) 

Instance Method

# commitEditing(withDelegate:didCommit:contextInfo:)

Attempt to commit any currently edited results of the receiver.

macOS 10.5+

``` source
@MainActor
func commitEditing(
    withDelegate delegate: Any?,
    didCommit didCommitSelector: Selector?,
    contextInfo: UnsafeMutableRawPointer?
)
```

## Parameters 

`delegate`  

An object that can serve as the receiver’s delegate. It should implement the method specified by `didCommitSelector`.

`didCommitSelector`  

A selector that is invoked on delegate.

`contextInfo`  

Contextual information that is sent as the `contextInfo` argument to delegate when `didCommitSelector` is invoked.

## Discussion

The receiver must have been registered as the editor of an object using objectDidBeginEditing:, and has not yet been unregistered by a subsequent invocation of objectDidEndEditing:. When the committing has either succeeded or failed, send the `delegate` the message specified by `didCommitSelector`.

The `didCommitSelector` method must have the following method signature:.

```
- (void)editor:(id)editor didCommit:(BOOL)didCommit contextInfo:(void  *)contextInfo
```

If an error occurs while attempting to commit, for example if key-value coding validation fails, an implementation of this method should typically send the receiver’s view apresentError(_:modalFor:delegate:didPresent:contextInfo:) message, specifying the view’s containing window.

You may find this method useful in some situations when you want to ensure that pending changes are applied before a change in user interface state. For example, you may need to ensure that changes pending in a text field are applied before a window is closed. See also commitEditing() which performs a similar function but which allows you to handle any errors directly, although it provides no information beyond simple success/failure.

## See Also

### NSEditor Conformance

func commitEditing() -> Bool

Returns whether the receiver was able to commit any pending edits.

func discardEditing()

Causes the receiver to discard any changes, restoring the previous values.

