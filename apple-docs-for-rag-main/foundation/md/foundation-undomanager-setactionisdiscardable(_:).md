

- Foundation
- UndoManager
-  setActionIsDiscardable(\_:) 

Instance Method

# setActionIsDiscardable(\_:)

Sets whether the next undo or redo action is discardable.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func setActionIsDiscardable(_ discardable: Bool)
```

## Parameters 

`discardable`  

Specifies if the action is discardable. true if the next undo or redo action can be discarded; false otherwise.

## Discussion

Specifies that the latest undo action may be safely discarded when a document can not be saved for any reason.

An example might be an undo action that changes the viewable area of a document.

To find out if an undo group contains only discardable actions, look for the `NSUndoManagerGroupIsDiscardableKey` in the userInfo dictionary of the NSUndoManagerWillCloseUndoGroup.

## See Also

### Using discardable undo and redo actions

var undoActionIsDiscardable: Bool

A Boolean value that indicates whether the next undo action is discardable.

var redoActionIsDiscardable: Bool

A Boolean value that indicates whether the next redo action is discardable.

