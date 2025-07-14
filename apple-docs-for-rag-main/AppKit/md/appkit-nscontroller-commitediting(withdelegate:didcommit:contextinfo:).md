

- AppKit
- NSController
-  commitEditing(withDelegate:didCommit:contextInfo:) 

Instance Method

# commitEditing(withDelegate:didCommit:contextInfo:)

Attempts to commit any pending changes in known editors of the receiver.

macOS

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

A selector that is invoked on delegate. The method specified by the selector must have the same signature as the following method:

```
- (void)editor:(id)editor didCommit:(BOOL)didCommit contextInfo:(void  *)contextInfo
```

`contextInfo`  

Contextual information that is sent as the `contextInfo` argument to delegate when `didCommitSelector` is invoked.

## Discussion

Provides support for the NSEditor informal protocol. This method attempts to commit pending changes in known editors. Known editors are either instances of a subclass of `NSController` or (more rarely) user interface controls that may contain pending edits—such as text fields—that registered with the context using objectDidBeginEditing(_:) and have not yet unregistered using a subsequent invocation of objectDidEndEditing(_:).

The receiver iterates through the array of its known editors and invokes `commitEditing` on each. The receiver then sends the message specified by the `didCommitSelector` selector to the specified delegate.

The `didCommit` argument is the value returned by the editor specified by `editor` from the `commitEditing` message. The `contextInfo` argument is the same value specified as the `contextInfo` parameter—you may use this value however you wish.

If an error occurs while attempting to commit, for example if key-value coding validation fails, your implementation of this method should typically send the view in which editing is being performed a `presentError:modalForWindow:delegate:didRecoverSelector:contextInfo:` message, specifying the view’s containing window.

You may find this method useful in some situations (typically if you are using Cocoa Bindings) when you want to ensure that pending changes are applied before a change in user interface state. For example, you may need to ensure that changes pending in a text field are applied before a window is closed. See also commitEditing() which performs a similar function but which allows you to handle any errors directly, although it provides no information beyond simple success/failure.

## See Also

### Managing editing

func objectDidBeginEditing(any NSEditor)

Invoked to inform the receiver that `editor` has uncommitted changes that can affect the receiver.

func objectDidEndEditing(any NSEditor)

Invoked to inform the receiver that `editor` has committed or discarded its changes.

func commitEditing() -> Bool

Causes the receiver to attempt to commit any pending edits, returning true if successful or no edits were pending.

func discardEditing()

Discards any pending changes by registered editors.

var isEditing: Bool

A Boolean value indicating if any editors are registered with the controller.

