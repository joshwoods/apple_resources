

- AppKit
- NSWindowDelegate
-  windowWillReturnUndoManager(\_:) 

Instance Method

# windowWillReturnUndoManager(\_:)

Tells the delegate that the window’s undo manager has been requested. Returns the appropriate undo manager for the window.

macOS 10.0+

``` source
@MainActor
optional func windowWillReturnUndoManager(_ window: NSWindow) -> UndoManager?
```

## Parameters 

`window`  

The window whose undo manager is being requested.

## Return Value

The appropriate undo manager for the specified window.

## Discussion

If this method is not implemented by the delegate, the window creates anUndoManager for `window`. Further, after a window creates its own undo manager, this method is never again called on the delegate.

